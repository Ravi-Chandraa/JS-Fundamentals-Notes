# JS-Fundamentals-Notes

Promises
The Promise object is used for deferred and asynchronous computations. A Promise represents a value which may be available now, or in the future, or never.

It has three states:

Pending
Fulfilled
Rejected
Looking at this piece of code:

new Promise((resolveOuter) => {
  resolveOuter(
    new Promise((resolveInner) => {
      setTimeout(resolveInner, 1000);
    })
  );
});
Chaining
When a promise becomes settled, you can use some of its methods to do further action: .then(), .catch(), and .finally().
555
666
888
999
