1、如果final修饰一个基本类型变量，表示这个变量是常量，一经赋值就不能再修改了，如果修饰的是一个引用，那这个引用不能够再引用其他对象，但是对象是可以修改的；

2、如果方法被final修饰，表示这个方法在子类当中不能够被重写；

3、如果final修饰一个类，这个类不能被继承，String类不能被继承就是因为String类被final修饰的；