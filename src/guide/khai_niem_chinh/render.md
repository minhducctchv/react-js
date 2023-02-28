# Việc render các element

Element là những mảnh ghép nhỏ nhất của các ứng dụng React.
```tsx
const element = <h1>Hello, world</h1>;
```

## Việc render một element vào trong DOM
Các ứng dụng React thường có 1 DOM gốc
```html
<div id="root"></div>
```
Dùng [ReactDOM.render](https://vi.reactjs.org/docs/react-dom.html#render) để truyền element vào DOM
```html
const element = <h1>Hello, world</h1>;
ReactDOM.render(element, document.getElementById('root'));
```

## Việc cập nhật element đã được render
React element là bất biến (ko thể thay đổi các children và các attribute của nó).
Các duy nhất để update "giao diện" (UI) là truyền nó vào [ReactDOM.render()](https://vi.reactjs.org/docs/react-dom.html#render)
```tsx
function tick() {
  const element = (
    <div>
      <h1>Hello, world!</h1>
      <h2>It is {new Date().toLocaleTimeString()}.</h2>
    </div>
  );
  ReactDOM.render(element, document.getElementById('root'));
}

setInterval(tick, 1000);
```

## React Chỉ Cập Nhật Những Gì Cần Thiết
ReactDOM sẽ so sánh element và các thành phần con của nó, chỉ cập nhật những element con thay đổi