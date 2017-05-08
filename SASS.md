# SASS Styling Guidelines

## 1. Naming conventions
### 1.1 Seperation
We use `-` as separators (don't camelCase or sneak_case).
`.my-awesome-classname`

### 1.2 Usefull names
Every time use fullnames for classed or identifiers.

````sass
.container
{
    // Some stylings
}

#vote
{
    // Some stylings	
}
````

## 2. Curly braces
As in PHP and JavaScript, we set curly braces on the next line.

````sass
.container
{
    // Some stylings
}

#vote
{
    // Some stylings
}
````
 
## 3. Basic structure
Image an HTML element always as a box. We order our CSS properties from outside to inside, followed by importance of the property.

 ````sass
.container
{
    // Basic positions, overflows
    position: absolute;
    display: block;
    
    overflow: hidden;
    
    // Position, Sizes
    top: 10px;
    left: 10px;
    
    height: 100px;
    width: 100px;
    
    // Fonts, Text, Colors
	font-family: 'Times New Roman', Georgia, Serif;
	font-weight: 300;
	
	text-decoration: none;
	
	color: #f0f0f0;
	
	// Margin, Paddings
	margin: 0;
	padding: 20px;
	padding-bottom: 0;
	
	// Borders, Background
	border: 1px solid black;
	background: #ffffff;
	
	// Index, various
	z-index: 1;
}
````

## 4. Nesting
Don't nest more than 3 levels

````sass
#my-awesome-component
{
    .frontrow
    {
        a.green
        {
             // Dont nest more
             
             &:hover
             {
	             // Don't do this
             }
        }
        
        a.green:hover
        {
            // Do this instead	        
        }
    }
}
````