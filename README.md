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

####Bootstrap Default Styles 
- <p> font size: 14px, line-height: 20px, Helvetica

####Definition Lists (HTML) 
- Use <dl> definition list <dt> def term <dd> def description
- Creates a list styled for word definition 
- Bootstrap class will make it horizontal, like a table  

####Table Structure 
<table> <caption> <thead> <tr> <th> <tbody> <tr> <td> 