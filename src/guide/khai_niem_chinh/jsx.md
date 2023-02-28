# Giới thiệu JSX

VD:
```tsx
const element = <h1>Hello, world!</h1>;
```

## Tại sao lại là JSX?
bla bla...

## Nhúng Biểu thức trong JSX

- dùng dấu ngoặc nhọn `{}`
```tsx
const name = 'Josh Perez';
const element = <h1>Hello, {name}</h1>;
```
- dút đc [tất cả các biểu thức hợp lệ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#Expressions)

## JSX cũng là một biểu thức

có thể dùng jsx trong code js, gán cho biến dùng, trong `if`, dùng trong `for`

## Xác định thuộc tính của thẻ với JSX

dùng dấu `""` cho giá trị thuộc tính string
```tsx
const element = <div tabIndex="0"></div>;
```
dùng `{}` cho giá trị thuộc tính biểu thức JS
```tsx
const element = <img src={user.avatarUrl}></img>;
```
:::warning CẢNH BÁO
JSX dùng `camelCase` cho thuộc tính thay vì dùng tên gốc HTML.
VD: `tabindex` => `tabIndex`
:::
## Dùng thẻ con trong JSX
`<thẻCha>` có thể chứa nhiều `<thẻCon>` giống HTML

## JSX chống tấn công kiểu Injection
bal bal...

## JSX là đối tượng
Babel biên dich JSX thành code JS `React.createElement(...)`

:::tip Gợi ý
Nên [cấu hình babel](https://babeljs.io/docs/en/next/editors) cho IDE để code ES6 và JSX được format
:::
