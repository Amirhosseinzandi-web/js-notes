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
