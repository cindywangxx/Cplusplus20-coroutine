# Cplusplus20-coroutine
# contents about C++ 20 coroutine

The C++ standards committee publishes experimental C++ language and library extensions for future standardization
#import <experimental/coroutine>

coroutine三个关键字：co_await, co_yield, co_return

1: co_await
co_await 是个操作符，完成操作符重载就可以实现coroutine等待任何类型。重载函数返回类型需要定义三个函数： 
bool await_ready(T& )nonexcept{}
void await_suspend(T&, std::experimental::coroutine_handle<T>)nonexcept{}
void await_resume(T& )nonexcept{}



