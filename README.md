# Prepare environment

1. Create new HTML Page
2. Add script reference to your go.js file
3. Add DIV element for diagram
4. Define body onload function

# Create Diagram, Model and Model Data

### 1. Store go.GraphObject.make in simple variable (such as $)

### 2. Define myDiagram as a new Diagram

- First argument: go.Diagram
- Second argument: ID of the DIV element our diagram should be associated with

### 3. Set Diagram height, width, and border

### 4. Create nodeDataArray and linkDataArray (each element is an object in JSON format)

- nodeDataArray-> Only contains a string value for the "key" property (unique property that acts as an identifier for each Node in GoJS)
- linkDataArray-> We'll have a single element, with two properties: "to" and "from" (keys of the nodes this link connects)

### 5. Set Diagram.model

# Create Node Template

### 1. Define node templates as a single "Auto" Panel

### 2. Define node template elements (Shape and TextBlock)

### 3. Add color data property to nodes in nodeDataArray

### 4. Add node data bindings

# Create Link Template

### 1. Define link template with two Shape elements

### 2. Add link data bindings

# Edit Node / Link Properties

### 1. Set margin propert on nodeTemplate's Shape element

### 2. Set strokeWidth property linkTemplate's first Shape element

- ! Organizing Nodes and Links together is made easy with Groups
- Groups will treat a collection of Nodes and Links as though they were a single Node
- We can create a group by adding a new element in the noddeDataArray

# Create a group

### 1. Add Group data to nodeDataArray

### 2. Add new nodes in nodeDataArray and ser "group" property

### 3. Add link to Group in linkDataArray
