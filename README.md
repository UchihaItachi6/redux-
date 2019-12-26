# redux-

(1)Redux  实例称为 store 并用以下方式创建：
    import { createStore } from 'redux'
    var store = createStore(() => {})
    也可以这样写：
    const reducer = (state= 5) =>{
       return state;
    }
    let store = Redux.createStore(reducer);
   createStore 函数必须接收一个能够修改应用状态的函数。
   redux可以用getState()方法检索 Redux store 对象中保存的当前的state。
   let getstore =  store.getState();
   
(2) 在 Redux 中，所有状态更新都由 dispatch action 触发, action 必须带有type属性，该属性表示此 action 的类型。
     let action = {
      type:'LOGIN'
     }
    
(3) Reducer 函数只是一个纯函数，它接收应用程序的当前状态以及发生的 action，然后返回修改后的新状态（或者有人称之为归并后的状态）。

