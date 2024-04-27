# js-notes
<h1>یکسری نکات و توضیحات برای Js</h1>
<hr/>
<h3>_ لودینگ مصنوعی با Promis</h3>
<pre>
  function fakeLoading() {
  return new Promise((resolve, reject) => {
    // Simulate a loading process
    setTimeout(() => {
      resolve(); // Resolve the promise after a certain delay
    }, 2000); // Delay of 2 seconds
  });
}

// Usage
fakeLoading()
  .then(() => {
    console.log('Loading complete!');
  })
  .catch((error) => {
    console.error('Error during loading:', error);
  });
</pre>
</hr>
<h3>متد Splice</h3>
<pre>
let arr = [15 , 20 , 25];
let arr1 = arr.splice(1);
console.log(arr1);
</pre>
<p>از اندیس 1 شروع میکنه به حذف و به عنوان خروجی ، آرایه ای میده از عناصر حذف شده.</p>
