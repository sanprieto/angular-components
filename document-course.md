# document course
## @Input
Se utiliza para pasar datos desde un componente parent a un child.

*Nota: Es necesario el decorador:  Import {@Input}*
- Child component, typescript:
```typescript
@Input() img: string = ''
```
- Child component, html:
```html
<img width="150" [src]="img">
```
- Parent component, typescript:
```typescript
export class AppComponent {
  imgParent = 'https://www.w3schools.com/howto/img_avatar.png';
}
```
- Child component, html:
```html
<app-img [img]="imgParent"></app-img>
```

