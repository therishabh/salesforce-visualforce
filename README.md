# Salesforce Visualforce

## What is Visualforce ?
- Visualforce is the component-based user interface framework for the Force.com platform.
- The framework includes a tag-based markup language, similar to HTML. So just like in HTML we have tags like <body> tag and p tag etc. Similarly in visualforce we have tags.
- A web development framework that allows you to create custom user interfaces that can be used in the Lightning Platform
- Each Visualforce page can be accessible by a unique URL
- Visualforce Page uses tag based markup which is similar to HTML. Each tag has its own properties and corresponds to a user interface element such a block, section, list, row, etc.
- Lot of flexibility as VF markup can easily be mixed with generic HTML, Javascript, CSS which in turn provides flexibility in creating custom screens for users.
- Visualfofce has nearly 150 built in components that you can use on the page to build custom screens & pages.

### When you should use Visualforce ?
Visualforce consists of a tag-based markup language that gives developers a more powerful way of building applications and customizing the Salesforce user interface. With Visualforce you can:
- You can override the standard salesforce pages with Visualforce page.
- Create your own custom flow control through an application.
- Define navigation patterns and data-specific rules for optimal, efficient application interaction.

### Advantages of Visualforce
- Visualforce is a Model View Controller (MVC) development style.
- Visualforce Editor panel is present for every visualforce page.
- Visualforce has Huge number of components.
- Can be integrated with HTML, CSS, Ajax, Query.
- Visualforce is flexible and customizable with web technologies.

### Visualforce tags can be divided to different types:
- Input tags
- Output tags
- Select tags
- Form tags
- Page tags
- Action tags
- Style tags

## Page Tags
**Visualforce Page tags:**
- <apex:page>
- <apex:pageMessage>
- <apex:pageBlock>
- <apex:pageBlocktable>
- <apex:pageBlockButtons>
- <apex:pageBlockSectionItem>

### <apex:page>
The basic tag that creates a visualforce page. **Can be used only once in a page** and all visulforce Tags **have to be enclosed in this tag**.

```java
<apex:page>
  <h1>Hello Title </h1>
</apex:page>
```

### apex:pageblock
A tag that creates an area within the page where multiple sections can be created and fields, buttons, tables or links can be displayed. It by default inherits the standard salesforce page style.

### apex: pageBlockSection
This tag helps to create a section inside a page block.
Multiple sections can be created in a page block and each section can be used to display any fields (input/output).

```html
<apex:page>
   <apex:pageBlock title="Block One">
    <apex:pageBlockSection title="Section One Title" columns="3">
       <apex:pageBlockSectionItem labelTitle="item1 title">Item 1 here</apex:pageBlockSectionItem>
       <apex:pageBlockSectionItem labelTitle="item2 title">Item 2 here</apex:pageBlockSectionItem>
       <apex:pageBlockSectionItem labelTitle="item3 title">Item 3 here</apex:pageBlockSectionItem>
     </apex:pageBlockSection>
       <apex:pageBlockSection title="Section Two Title" columns="4">
       <apex:pageBlockSectionItem labelTitle="item1 title">Item 1 here</apex:pageBlockSectionItem>
       <apex:pageBlockSectionItem labelTitle="item2 title">Item 2 here</apex:pageBlockSectionItem>
       <apex:pageBlockSectionItem labelTitle="item3 title">Item 3 here</apex:pageBlockSectionItem>
       <apex:pageBlockSectionItem labelTitle="item4 title">Item 4 here</apex:pageBlockSectionItem>
       </apex:pageBlockSection>
   </apex:pageBlock>
</apex:page>
```

### apex:pageBlockButton
Whenever < apex:commandbutton> tag is used, a button is created in a based on the position where the tag is written. But most of the times, we may want to place the buttons on the top or bottom of the page. This can be achieved with the help of this tag.


### apex:pageMeaage
This component should be used for presenting custom messages in the page using the Salesforce pattern for errors, warnings and other types of messages for a given severity. See also the pageMessages component.
There is one required attribute for this tag named Severity.

Severity: The severity of the message. 
**Severity:**  Values supported are: 'confirm', 'info', 'warning', 'error' 
**Strength:** The strength of the message. This controls the visibility and size of the icon displayed next to the message. Use 0 for no image, or 1-3 (highest strength, largest icon).

```html
<apex:page>
<apex:pageBlock>
    <apex:pageMessage summary="validation message" severity="confirm" strength="2"></apex:pageMessage>
</apex:pageBlock>
</apex:page>
```

![Screenshot 2024-05-17 at 3 21 45 AM](https://github.com/therishabh/salesforce-visualforce/assets/7955435/2da064b3-3803-48fc-afca-472d63b6232a)


### Input Tags
Input tags used to capture user input for any standard or custom object field, and respects any metadata that is set on the field definition, such as whether the field is required or unique, or whether the current user has permission to view or edit it.
Example of input tags:
```html
- <apex:inputsecret>
- <apex:inputcheckbox>
- <apex:inputFile>
- <apex:inputHidden>
- <apex:inputField>
- <apex:inputTextArea>
```

## Output tag and OutputLink tag
**<apex:outputLabel> :** <br/>
A label for an input or output field. Use this component to provide a label for a controller method that does not correspond to a field on a Salesforce object.<br/><br/>
**<apex:outputLink>:**<br/>
This tag creates a link to a URL. The below code displays the text www.salesforce.com as a hyperlink text on the visual force page and when this link is clicked the URL specified in the value attribute will be opened. The body of an < apex:outputLink > can be text or an image


#### Q. What is the architechture of Salesforce ? or MVC Architecture ?
Ans : <br/>
![Screenshot 2024-06-09 at 2 26 49 AM](https://github.com/therishabh/salesforce-visualforce/assets/7955435/3a18b497-1a43-4bb6-8f37-90eea9a03eb1)

Detailed examples:<br/><br/>
Examples of M : (Model)<br/>
object, Relationship, Field etc<br/><br/>
Examples of V: (View)<br/>
Logo, Tab, Button, Link, Page layout, Visualforce page etc<br/><br/>
Examples of C: (Controller)<br/>
APEX code, WER, PB, Trigger, VR, AP etc<br/><br/>

IQ: TCS
#### Q. What is force.com ? <br/>
Ans : <br/>
Force.com = platform<br/>
Salesforce.com = software (SFDC)<br/><br/>
(but everything belongs to company Salesforce)<br/><br/>

Force.com is example of PAAS<br/>
Salesforce.com is example of SAAS<br/>
(IAAS = not useful for our career)<br/>



















