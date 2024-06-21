### 一、模板

#### 1.1 函数模板



```c++
#include <iostream>
#include <string>
#include <fstream>
using namespace std;

// 告诉编译器，T是个数据类型，后续使用别报错
template<class T> 
void MySwap(T& a, T& b)
{
	T temp = a;
	a = b;
	b = temp;
}

// 在哪一个函数上写模板，这个模板就是那个函数的专属
// 其他函数使用，得重新定义
template<class T> 
void func() {

}

int main()
{
	func<double>();
	
   return 0;
}
```

















