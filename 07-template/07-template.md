��������ҪΧ����ģ��չ���������Ǽ�¼��һЩ֪ʶ��


# ����
Concepts��C++20���������ԣ�����һ��ν�ʣ�����Լ��ģ������Ͳ���Ӧ�þ��е����ԡ�  
�� ���� Comparable T ��˵��ģ������Ͳ��� Ӧ���ǿɱȽϵġ�
## ����Ĺ�������
~~~cpp
template<typename T>
concept Comparable = requires(T a, T b){
{a < b} -> std::convertiable_to(bool)
};
~~~

## ʹ�ø���Լ��ģ��
~~~cpp
template<Comparable T>
void compare(T a, T b)
{
  if(a < b)
	std::cout<<"a<b\n";
  else
	std::cout<<"a>b\n";
}
~~~

## ʹ�ñ�����Լ����ģ�庯��
~~~cpp
int main()
{
	int a=1, b=2;
	compare(a, b);
}
~~~
���Ͼ��Ǹ�������ݡ�


