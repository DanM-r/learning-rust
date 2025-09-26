# Smart Pointers

A reference in rust is a pointer. Smart pointers are data structures of a pointer with metadata and added caapabilities.

Smart pointers usually are owners.

`String` and `Vec<T>` are considered smart pointers.

Implemented with structs with `Deref` and `Drop` traits.

- `Deref`: add reference behaviour
- `Drop`: customize code when an instance of a smart pointer goes out of scope.

Most common smart pointers:

- `Box<T>`: allocation in heap.
- `Rc<T>`: reference counting, multiple ownership.
. `Ref<T>` and `RefMut<T>` accessed trough `RefCell<T>`: enforces borrowing at runtime instead of compile time.

## Type `Box<T>`

No performance overhead.

Uses:

- No size at compile time