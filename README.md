# modify-materialUI-components-style
How to modify angular material UI components styles guide

![Animation3](https://user-images.githubusercontent.com/95239629/143911449-29a36a84-3861-4540-822e-86e883bf5ec8.gif)
![Animation](https://user-images.githubusercontent.com/95239629/143911457-cc55be21-00d1-4075-94eb-b9a3723864f2.gif)
![Animation2](https://user-images.githubusercontent.com/95239629/143911462-9bc4bc80-a9a0-4e68-9e67-48fe1d575431.gif)

##  Use ::ng-deep to shadow peirce
::ng-deep selector
Component styles normally apply only to the HTML in the component's own template.

Use the ::ng-deep shadow-piercing descendant combinator to force a style down through the child component tree into all the child component views. The ::ng-deep combinator works to any depth of nested components, and it applies to both the view children and content children of the component.

```::ng-deep h3 {
  font-style: italic;
}```

The ::ng-deep combinator also has the aliases >>>, and /deep/.

Use /deep/, >>> and ::ng-deep only with emulated view encapsulation. Emulated is the default and most commonly used view encapsulation. For more information, see the view encapsulation section.

The shadow-piercing descendant combinator is deprecated and support is being removed from major browsers and tools. As such we plan to drop support in Angular (for all 3 of /deep/, >>> and ::ng-deep). Until then ::ng-deep should be preferred for a broader compatibility with the tools.

## Useful links to study further

* [Change background color for Angular Material mat-select component](https://pretagteam.com/question/change-background-color-for-angular-material-matselect-component)
* [Angular Material - Change color of mat-list-option on selected](https://newbedev.com/angular-material-change-color-of-mat-list-option-on-selected)
* [Angular Material Pagination select color change to none?](https://stackoverflow.com/questions/43903828/angular-material-pagination-select-color-change-to-none?rq=1)
