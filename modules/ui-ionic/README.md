# ng2 Dynamic Forms Ionic UI

## Installation
```
npm install @ng2-dynamic-forms/ui-ionic -S
```

## Import
```ts
@NgModule({

    imports: [
        // ...
        ReactiveFormsModule,
        DynamicFormsCoreModule.forRoot(),
        DynamicFormsIonicUIModule
    ]
})

export class AppModule {}
```

## Usage

with **`DynamicIonicFormComponent`**:
```ts
<form [formGroup]="myFormGroup">

    <dynamic-ionic-form [group]="myFormGroup"
                        [model]="myFormModel"></dynamic-ionic-form>
</form>
```

with **`DynamicIonicFormControlComponent`**:
```ts
<form [formGroup]="myFormGroup">

    <dynamic-ionic-form-control *ngFor="let controlModel of myFormModel"
                                [group]="myFormGroup"
                                [model]="controlModel"></dynamic-ionic-form-control>
</form>
```

## Form Controls

|                                  Control                                  	|                        Model                       	| Required Property 	|
|:-------------------------------------------------------------------------:	|:--------------------------------------------------:	|:-----------------:	|
|    **[Checkbox](http://ionicframework.com/docs/components/#checkbox)**    	| `DynamicCheckboxModel`                             	|         –         	|
| **[Checkbox Group](http://ionicframework.com/docs/components/#checkbox)** 	| `DynamicCheckboxGroupModel`                        	|         –         	|
|    **[DateTime](http://ionicframework.com/docs/components/#datetime)**    	| `DynamicDatePickerModel`, `DynamicTimePickerModel` 	|         –         	|
|       **[Input](http://ionicframework.com/docs/components/#inputs)**      	| `DynamicInputModel`                                	|         –         	|
|    **[Radio Group](http://ionicframework.com/docs/components/#radio)**    	| `DynamicRadioGroupModel`                           	|         –         	|
|       **[Range](http://ionicframework.com/docs/components/#range)**       	| `DynamicSliderModel`                               	|         –         	|
|      **[Select](http://ionicframework.com/docs/components/#select)**      	| `DynamicSelectModel`                               	|         –         	|
|     **[TextArea](http://ionicframework.com/docs/components/#inputs)**     	| `DynamicTextAreaModel`                             	|         –         	|
|      **[Toggle](http://ionicframework.com/docs/components/#toggle)**      	| `DynamicSwitchModel`                               	|         –         	|