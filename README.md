# class-templates
Class templates with typenames for variables. Including a vector of template classes with double as the template parameters.
There is also a template class, called My_pair that uses two typename variables, T1 and T2.

This code  would of course typically be contained in .header files. But given this is a github portfolio file I have kept it a part of the main.cpp file.
The class Item require's a string variable & uses T value as the template parameter.

T get_value() const { return value; } //this getter returns value, value being determined by the parameters passed in to the template class.
Item <int> item1{ "Jenny", 100 }; //the 100 is the template T value.
Item <std::string> item2{ "Jenny", "Elizabeth" }; //the template will be passed a string as it's value parameter.
Item <Item<std::string>> item3{ "Jenny", {"Elizabeth", "Gabriel"} }; //item3's T value is another item with a passed in string and a Tvalue of it's own that is a string.
