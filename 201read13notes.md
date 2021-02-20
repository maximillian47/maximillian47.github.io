 Calling setItem() with a named key that already exists will silently overwrite the previous value. 
    
 Calling getItem() with a non-existent key will return null rather than throw an exception.

     \var foo = localStorage.getItem("bar");
     localStorage.setItem("bar", foo);

 Instead of using the getItem() and setItem() use square brackets:
   
     \var foo = localStorage["bar"];
     localStorage["bar"] = foo;

 Deleting all key:val pairs

     \interface Storage {
     deleter void removeItem(in DOMString key);
     void clear();
     };
 Getting total number of vals in storage and iterating through all keys by index

     interface Storage {
       readonly attribute unsigned long length;
       getter DOMString key(in unsigned long index);
     };
     
     
     
     function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}



let foo = localStorage.getItem('bar');
localStorage.setItem('bar', foo);

// removing the value for a given named key
interface Storage {
  deleter void removeItem(in DOMString key);
  void clear();
};

// get the total number of values in the storage area
interface Storage {
  readonly attribute unsigned long length;
  getter DOMString key(in unsigned long index);
};


if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};
