Be generous with your interfaces. Take as little as you need, give as much as you can.

Imagine getting a driver's license in a foreign country. You need a birth certificate, fingerprint, and proof of residency like a utility bill in your name. But you need a local bank account to get a utility bill and you need local ID to get a bank account...

And remember that driver's licenses don't actually drive cars. This is just to make your day less bad if you get pulled over.

The opposite of this is the ocean. The ocean gives salt water. What does the ocean ask of you to get water? As little as it can. If you want to take it with you, you need a container. Want to just swim at the beach? That's fine too. There's no `OceanReady` type check that subclasses from `HasContainer`.

A good code example is the iterator protocol in Python. Define `__iter__` and your class can do some cool stuff. It can be used in for loops, and tuple unpacking. It asks one specific thing of you and gives you a lot.

There are more. If you define `__len__` you can call `len()` on your class. If you define `__getitem__` you can use the square bracket syntax, `like_this[0]`. And if you do both and inherit from `collections.abc.Sequence`, you can also use `reversed`, check containment with `in`, you get `.index()` and `.count()` methods and, oh, everything from the iterator protocol I mentioned earlier. `Sequence` asks you to give two things and gives you five really good things back.

If you keep asking yourself "how little can I ask for and how much can I give?", it will lead you towards composition. `Sequence` is halfway up the inheritance tree in `collections.abc`. If you want a `MutableSequence`, you define three more methods and get six more back.

I know complex class hierarchies scare people, and they should. I think that's because we're often using them to make taxonomies. They're pretty bad for that, despite what your introduction to OOP might have said. Dogs don't "extend" Mammal, they don't extend Wolf. They're their own thing.

All of this also applies to functions. It's even easier.

Why try to be generous? It's not just to be nice. It's because control only gets you so far. People are out there implementing classes with dummy values for mandatory attributes. They're doing this because they still find the code useful. This means that they're right and whoever wrote the class was wrong about this thing being "mandatory".

If you want people to use your code in the way that you want, one path is to want less. When you can, try to not be like the DMV. Be like the ocean.
