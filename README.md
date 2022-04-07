#  telegram bot @themaltsev modified by @kittyyywr
___
The main modification is `localStorage.clear();`
```js

init(){  
    localStorage.clear();
    $('body').insertAdjacentHTML( 'afterbegin', tpl)
    let store = localStorage.getItem("historyMessages");

    if (store !== null) {
      $('.chat__body').innerHTML = store
    }

    $('.chat__main__input').addEventListener('keypress', (e)=>{

      if(e.key === `Enter`) this.submit();

    })

    $(".chat__input__submit").onclick = () => this.submit();

    

  }
```
## How to install a widget on your site see here->
[CLICK](https://www.youtube.com/watch?v=qFpcITfjpe8)
