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
مثال 1 : 
let arr = [15 , 20 , 25 , 47 , 53];
let arr1 = arr.splice(1);
console.log(arr1); // [20 , 25 , 47 , 53]
</pre>
<p>از اندیس 1 شروع میکنه به حذف و به عنوان خروجی ، آرایه ای میده از عناصر حذف شده.</p>
<pre>
مثال 2 : 
let arr = [15 , 20 , 25];
let arr1 = arr.splice(1,1);
console.log(arr1); // [20]
</pre>
<p>اندیس اول ، اندیس شروع و اندیس دوم ، تعداد عناصری که باید حذف شوند است. از اندیس اول ، یک عنصر حذف میشود و سپس خروجی ، آرایه از عناصر حذف شده است یعنی [20]</p>

