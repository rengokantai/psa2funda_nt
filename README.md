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

### Lazily Loading Feature
submodule->CommonModule
appmoeule->BrowserModule
