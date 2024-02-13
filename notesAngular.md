# Angular :

### Notion vue jour 1 : 
# les ng-directives :
#### - *ngif : utiliser pour afficher ou cacher un élément en fonction d'une condition,  : `<div *ngIf="condition">Contenu</div>`.
#### - *ngFor : utiliser pour afficher une liste d'éléments:
`<div *ngFor="let item of items"> {{item}} </div>`.
#### - *ngSwitch : utiliser pour afficher un élément en fonction d'une condition :
#### `<div [ngSwitch]="condition"> <div *ngSwitchCase="1">Contenu 1</div><div *ngSwitchCase="2">Contenu 2</div><div *ngSwitchDefault>Contenu par défaut</div>`

#### - [ngStyle] : utiliser pour appliquer un style en fonction d'une condition:
#### `<div [ngStyle]="{'color': condition ? 'red' : 'blue'}">Contenu</div>`.
#### - [ngClass] : utiliser pour appliquer une classe en fonction d'une condition : 
#### `<div [ngClass]="{'class1': condition, 'class2': !condition}">Contenu</div>`.
#### - [ngModel] : utiliser pour lier un input à une variable :
#### `<input [(ngModel)]="variable">`.
#### - [ngForm] : utiliser pour lier un formulaire à une variable:
#### `<form [ngForm]="variable">Contenu</form>`.
# Les events :
#### - (click) : utiliser pour déclencher une fonction lors d'un click :
#### `<button (click)="fonction()">Bouton</button>`.
#### - (input) : utiliser pour déclencher une fonction lors d'un input :
#### `<input (input)="fonction()">`.
#### - (change) : utiliser pour déclencher une fonction lors d'un changement : 
#### `<input (change)="fonction()">`.
#### - (submit) : utiliser pour déclencher une fonction lors d'un submit :
#### `<form (submit)="fonction()">Contenu</form>`.
#### - (keyup) : utiliser pour déclencher une fonction lors d'un relâchement d'une touche :
#### `<input (keyup)="fonction()">`.
#### - (keyup.enter) : utiliser pour déclencher une fonction lors d'un relâchement de la touche entré :
#### `<input (keyup.enter)="fonction()">`.
# Les attributs :
#### - [hidden] : utiliser pour cacher un élément :
#### `<div [hidden]="condition">Contenu</div>`.
#### - [disabled] : utiliser pour désactiver un élément :
#### `<button [disabled]="condition">Bouton</button>`.
#### - [value] : utiliser pour définir la valeur d'un élément :
#### `<input [value]="valeur">`.

# Specialement pour les formulaires :
#### - [formControl] : utiliser pour lier un input à un formControl :
#### `<input [formControl]="formControl">`.
#### - [formGroup] : utiliser pour lier un formulaire à un formGroup :
#### `<form [formGroup]="formGroup">Contenu</form>`.
#### - [formArrayName] : utiliser pour lier un formulaire à un formArray :
#### `<div [formArrayName]="formArray">Contenu</div>`.
#### - [formControlName] : utiliser pour lier un input à un formControl 
#### `<input [formControlName]="formControl">`.
#### - [formGroupName] : utiliser pour lier un groupe d'input à un formGroup 
#### `<div [formGroupName]="formGroup">Contenu</div>`.

# Les pipes :
#### - uppercase : utiliser pour mettre en majuscule une chaine de caractère :
#### exemple : `{{'chaine' | uppercase}}`.
#### - lowercase : utiliser pour mettre en minuscule une chaine de caractère :
####  `{{'CHAINE' | lowercase}}`.
#### - titlecase : utiliser pour mettre en majuscule la première lettre de chaque mot :
####  `{{'chaine de caractère' | titlecase}}`.
#### - slice : utiliser pour extraire une partie d'une chaine de caractère:
####  `{{'chaine de caractère' | slice:0:5}}`.
#### - json : utiliser pour afficher un objet en format json :
####  `{{objet | json}}`.
#### - date : utiliser pour formater une date : 
####  `{{date | date:'dd/MM/yyyy'}}`.
#### - currency : utiliser pour formater un nombre en monnaie 
####  `{{nombre | currency:'EUR'}}`.
#### - percent : utiliser pour formater un nombre en pourcentage 
####  `{{nombre | percent}}`.
#### - async : utiliser pour afficher le résultat d'un observable : 
####  `{{observable | async}}`.

# Les services :
#### - HttpClient : utiliser pour faire des requêtes http : 
#### `this.http.get('url').subscribe((data) => { console.log(data); });`.
#### - Router : utiliser pour naviguer entre les pages 
#### `this.router.navigate(['url']);`.
#### - ActivatedRoute : utiliser pour récupérer les paramètres de l'url : 
#### `this.route.snapshot.paramMap.get('parametre');`.
#### - FormBuilder : utiliser pour créer des formGroup et des formControl :
#### `this.formBuilder.group({formControl: ['valeur']});`.
#### - FormGroup : utiliser pour créer un groupe d'input : 
#### `this.formBuilder.group({formControl: ['valeur']});`.
#### - FormControl : utiliser pour créer un input 
#### `this.formBuilder.control('valeur');`.
#### - FormArray : utiliser pour créer un tableau d'input 
#### `this.formBuilder.array([this.formBuilder.control('valeur')]);`.

# Les observables :
#### - subscribe : utiliser pour écouter les changements d'un observable. exemple : `observable.subscribe((data) => { console.log(data); });`

### Notion vue jour 2 :
