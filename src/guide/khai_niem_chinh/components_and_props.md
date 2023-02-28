# Components và Props

Tìm hiểu chi tiết về component tại [đây](https://vi.reactjs.org/docs/react-component.html)

## Function Components và Class Components
### Function components
đây là khai báo component với props truyền vào kiểu function
```tsx
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```
### Class components
đây là khai báo component với props truyền vào kiểu [ES6 class](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Classes)
```tsx
class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```

chúng ta sẽ thảo luận về điểm khác biệt của chúng ở [phần tiếp theo](https://vi.reactjs.org/docs/state-and-lifecycle.html)

## Rendering một Component

## Tạo Components

## Tách Components

## Props chỉ dùng để đọc