# psa2funda_nt

## 6
### Pre-loading Data
```
Subject s = new Subject();
subject.map(events=>events)
```
#### 05:46
```
{path: 'events',component:EventListComponent,resolve:{events:EventListResolver}}
```

```
this.events = this.route.snapshot.data['events']
```

### Styling Active Links
```
<a [routerLink]="['/event']" routerLinkActtive="cls">
```

## 7.
### Creating Custom Validators
#### 05:09
```
private restrictedWords(words){
  return (control:FormControl):{[key:string]:any}=>{
  }
}
```

## 8. Communicating Between Components

### 2
```
[session]="event.sessions"]
```
I want to bind session propery of child component to session array of event object.




### Lazily Loading Feature
submodule->CommonModule
appmoeule->BrowserModule


#### 04:40
```
<a
```
```
{path:'user',loadChildren:'app/user/user.module#UserModule'
```

#### 04:23
```
<a [routerLink]="['user/profile']">
```

### Ahead of Time Compiler
AOT Benefits:
- Fast rendering
- Fewer Requests
- Smaller Angular Framework Download
- Detect Template Errors
- Better Security

Compilers:
- Development: Just in time compiler
- Production: Ahead of time Compiler

need to change to get aot work
```
declare let toastr: Toastr; -> let toastr:Toastr = window['toastr'];
```
```
newForm.controls.name?.invalid->newForm.form.ge('name')?.invalid
newForm.controls.firstName.errors.pattern->newForm.get('firstName').hasError('pattern')
```
