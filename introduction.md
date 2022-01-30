## Save your time

### Performance 

1. `Node is V8, C/C++, libuv, modules.`
    - V8 is fast because of C/C++ and engine runtime optimizations.
    - libuv is fast because of C/C++.
2. `Node is fast because of V8 and libuv`.
3. `Node is signle threaded.` But some of the native modules aren't (`crypto.pbkdf2`).
4. Almost all modules that use internally `libuv uv_queue_work()` are not single-threaded.
5. `UV_THREADPOOL_SIZE = 4` default value of the `libuv uv_queue_work()` multithreading.
6. 
