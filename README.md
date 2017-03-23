##Introduction to Bootstrap (Pluralsight: Scott Allen, 2013)

####Bootstrap Dependencies 
- basic styles depend on bootstrap css
- widgets require boostrap js 
- **Bootstrap js depends on jquery**
- in the BS dist file, keep the relationship between css and fonts (due to relative links). However, the js can be separated

####Core Concepts 
- **Semantic classnames** - names clearly convey the function of css classes  
- **Compositional** - Bootstrap classes are designed to be small, focused and easy to combine. This way, they don't force extra unwanted styles on the user  
- **Conventions** - BS styles rely on certain conventions; the classes must be applied to the correct HTML element

####Layout Concepts 
- Default behaviour: small columns will start to stack as the screen narrow. Wider columns will never break (a horizontal scroll bar will appear). 
- container (fixed): the container class will center all content on the page. It will stop columns stacking. In other words, the container has a fixed width, as does each column. 
- container-fluid: this will expand and contract to fill the device width. Each column will take up a fixed percentage of the container width. By itself, there will be no stacking and no horizontal scrolling. Pictures will resize but keep their aspect ratio. Text will reflow to fill its container. Column height may become mismatched. Some columns will become unusable.  
- responsive: the basic mechanism is media queries. These are built into BS. For example, the fixed with is 940px by default, but 1170px on a larger display. Using visible / hidden classes is also helpful.  

####Adding Your Own Styles 
1. search bootstrap.css for the style being applied
2. Copy into your own stylesheet and amend  

####Bootstrap Default Styles 
- <p> font size: 14px, line-height: 20px, Helvetica

####Definition Lists (HTML) 
- Use <dl> definition list <dt> def term <dd> def description
- Creates a list styled for word definition 
- Bootstrap class will make it horizontal, like a table  

####Table Structure 
- <table> <caption> <thead> <tr> <th> <tbody> <tr> <td> 
- Classes for <table>: table (full width), table-striped, table-bordered (subtle), table-hover (shading), table-condensed (reduce padding)

####Forms 
- By default, bootstrap styles forms as stacked (ie block level elements) with a fixed input width and some padding.  
- 'radio' and 'checkbox' classes align text to button
- 'input-mini', 'input-large' etc will size inputs. We can also use span sizes.  
- input class 'search' will create a rounded box 
- horizontal forms are more difficult: use <form class='form-horizontal'>, <div class="control-group"> and <label class='control-label'>. But we don't need to use tables. 
- span with class 'help-inline' can offer help text on a form  
- there are error classes to help with validation 

####Icons 
- bootstrap recommends the unpopular <i> element (supposed to be for italic text) for icons  
- but icon classes can also be added to span elements 
- font awesome has a larger selection of icons, optimized for bs 14px default font size  

