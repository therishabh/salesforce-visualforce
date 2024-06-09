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

---------------------------
![Screenshot 2024-05-17 at 3 21 45 AM](https://github.com/therishabh/salesforce-visualforce/assets/7955435/2da064b3-3803-48fc-afca-472d63b6232a)
---------------------------

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
<br/>
<br/>
Extra point:<br/><br/>
Whenever we do coding in SF, actually, indirectly we are working on Force.com platform<br/>
Dev console = Force.com IDE<br/><br/>
So we can conclude,<br/><br/>
admins/clients work on = salesforce.com layer<br/>
devs work on = salesforce.com and force.com layer<br/>


https://chromewebstore.google.com/detail/salesforce-advanced-code/lnkgcmpjkkkeffambkllliefdpjdklmi?hl=en&pli=1


#### Q. Why to use Visualforce page in project ?
Ans: <br/>
To work on complex pages.<br/><br/>
To display records from multiple objects.<br/><br/>
When we want more than 2 column display of data. (IQ)<br/><br/>
To edit multiple records at the same time.<br/><br/>
To create multiple records at the same time.<br/><br/>
Custom analytics capabilities.<br/><br/>
(Show some advance charts etc using JS code. Ex: Radar chart)<br/><br/>
Show lightning component in Classic page. (Bonus topic)<br/><br/>
Moral:<br/>
When u cant do the needed things in "declarative" mode (standard record page/form given by SF), then opt VFP.<br/><br/>

------------------------ 

IQ / JQ: IMP<br/>
Declarative / Config approach - working on project without code<br/>
Non declarative / Customization approach - working on project with code<br/><br/>
Admin syllabus = declarative<br/>
Dev syllabus = non declarative<br/>

#### What is VFP ?
A proprietary web development language created by Salesforce.com<br/>
Syntax for this language is like HTML.<br/>
Fits into the "View" level of MVC.<br/>
Allows developers to build custom web pages.<br/>
Not intended for pure custom website creation, only useful internal work of SF.<br/>
<br/>
Strength: It allows developers to easily create a complete custom page that has the exact look and feel like a "standard Salesforce page" <br/>


Every Visualforce page start with `<Apex:Page>`

![Screenshot 2024-06-09 at 5 05 58 AM](https://github.com/therishabh/salesforce-visualforce/assets/7955435/2e964d8e-bddf-4732-b581-a97b5eb7b0ff)

Create Visualforce Page:
![Screenshot 2024-06-09 at 5 08 15 AM](https://github.com/therishabh/salesforce-visualforce/assets/7955435/3b7f579f-20c7-458f-b777-a17e3fc6d0a9)


>> How you'll check is opened page is visualforce page or normal ordinary page, so for this we need to check in URL, if in URL /apex/ keyword exists that means it is visualforce page.

**Quiz: Fill in the blank**<br/>
The way, it's hard to imagine a Trigger without **xxxx** (which gives business logic to Irigger), on the same note, it's hard to imagine a VEP in RTP (real time project) without a "Controller"!!


**xxxx => Apex Class**

#### What is controller in VFP ?
The way APEX class gives "Business Logic" to Triggers.<br/>
Controller gives "Business Logic" + "Data" to VFP.<br/><br/>

> Controller is like a backbone of Visualforce page. because VFP itself is Dumb. it is completly depends on controller.

#### Types of Controllers in VFP ?

1. Standard controller
2. Custom Controller
3. Controller Extensions AKA Extensions

(controllers => Backbone!)

#### IQ: Controllers can be what?
#### Or
#### what entity can become controller?

1. Object (standard or custom)</br>
or</br>
2. Apex class</br></br>
Nothing else!!

#### Interviewer can ask you, tell me 2 reasons why we need visual force page ?
- Visualforce pages allow for the creation of custom user interfaces tailored to specific business needs.
- They enable the incorporation of custom logic and seamless integration with external systems.

#### why we need controller in visualforce page ? one line answer
A. Controllers are needed in Visualforce pages to handle business logic and manage data interactions between the user interface and Salesforce.

### Types of Controllers:
### 1. Standard Controllers :
- It deals with Standard as well as Custom objects.
- We can write the standard object name or custom object name as a parameter for fetching the records from the database
- They provide the standard functions like save,delete or create records.
- Standard controllers are very helpful in designing a UI for the (custom) pages
- Due to this, we can create a complete page with lessefforts using the controllers


**Syntax :**</br>
`<apex:page StandardController="Account">`     This is for accessing STANDARD OBJECT</br>
`<apex:page StandardController="Pen__c">`      This is for accessing CUSTOM OBJECT</br></br>

> As we know visual force page is kind of less used in the market in that way Standard controller is rarely used in the market. You can say standard controller almost useless because of some limitations 

**Standard controller :**
When our VFP is dependent on any controller which is actually an object (standard or custom, does not matter) then that controller is called as Standard Controller.<br/><br/>
Note: At a time, only 1 object can be used. Either standard or custom.

```apex
<apex:page standardController="Account">
    <apex:form>
        <apex:pageBlock title="My Content">
            <apex:pageBlockButtons>
            	<apex:commandButton action="{!save}" value="Save Me"/>
            </apex:pageBlockButtons>
            
            <apex:pageBlockSection title="My Content Section" columns="2"> 
                <apex:inputField value="{!Account.name}" required="false"></apex:inputField>
            	<apex:inputField value="{!Account.fax}" /> 
                <apex:inputField value="{!Account.phone}" />
            	<apex:inputField value="{!Account.accountNumber}"/> 
                <apex:inputField value="{!Account.industry}" />
            </apex:pageBlockSection>
        </apex:pageBlock>
    </apex:form>
</apex:page>
```

Output : 
<img width="1440"  alt="Screenshot 2024-06-09 at 6 23 44 AM" src="https://github.com/therishabh/salesforce-visualforce/assets/7955435/83614ae1-a1b4-4bcc-8c81-2629b6707c86">

![Screenshot 2024-06-09 at 5 57 02 AM](https://github.com/therishabh/salesforce-visualforce/assets/7955435/a668fcfb-78d0-47fd-831f-1688478ddf87)

Create a visualforce page tab and add it into our app.
<img width="1440" alt="Screenshot 2024-06-09 at 6 29 27 AM" src="https://github.com/therishabh/salesforce-visualforce/assets/7955435/d1bf9e2a-c339-430f-a352-c11cf2c961e8">

#### Issues with Standard Controller ?
1. We can not show data from multiple objects
2. We can not write our logic in some APEX class and call the same when button is pressed
3. We can not fetch data from database
4. We can not do any DML
5. Relationship data fetching process is not feasible.

...lots of limitations

### 2. Custom Controllers :
- These are written in a class, using apex code
- These are used when we cant perfoem the needed work using the standard controllers
- When we want additional functionality in the page, by processing the objects, we need to use Custom Controllers
- They are used to create rich Ul with complex data sets ete

**Syntax :** <br/>
`<apex:page Controller="MyControllersClass">` These dont use any object names as parameter.<br/><br/>

here,<br/>
MyControllersClass is an apex class which controls the VF actions and variables

**Example:**
```apex
<apex:page controller="ExampleClassForVFP">
    <apex:form>
    	<apex:pageBlock title="My Content">
        	<apex:pageBlockSection title="My Content Section" columns="2">
            	<apex:outputLabel>Enter Name: </apex:outputLabel>
                <apex:inputText value="{!userName}" />
                <apex:commandButton value="Click Me" Action="{!ShowMessage}"/>
                <apex:outputLabel>{!message}</apex:outputLabel>
            </apex:pageBlockSection>
        </apex:pageBlock>
    </apex:form>
</apex:page>
```

```apex
public class ExampleClassForVFP {
    public String userName {set;get;}
    public string message{set;get;}
    
    public void ShowMessage(){
        message = 'Welcome '+ userName;
    }
}
```

#### IQ: TCS
`<apex:inputText> Vs <apex:inputField>` ? <br/>
Ans:<br/>
**inputField -** "Copy" the field from that object which is mentioned as controller and display on a VE page | like сору paste work <br/>
**inputText -** it will help to create a field from scratch | stand alone field | new creation | not connected to any object.<br/>
<br/>
<br/>
Means, after using `<inputText>`, we have to take extra step like ######## to ensure data will go to DB, Which we don't need in case of `<inputField>`<br/><br/>
####### => DML
<br/>
<br/>
<br/>

#### IQ: Samsung
Benefits of using Command Button?<br/>
<br/>
1. After pressed, it will send VFP data to server (Sync concept)
2. It will call associated function
3. Update in dack wiem latest data present im server. it will bring fresh data! (Sync concept)


#### IQ: What are properties in Salesforce?
(the key players in the F'end to B'end and B'end to F'end transfer!)<br/><br/>
Set = we are giving rights to VFP to set values in the related variables present in APEX Class (frontend to backend) <br/><br/>
Get = we are giving rights to VFP to get values of the related variables on VFP present in APEX (backend to frontend) <br/><br/>
Example:<br/>
public string UserName {set;get;} <br/>
public string message {set; get;}<br/>
<br/>
<br/>
public string UserName {set;}<br/>
when error will come ?
<br/>
<br/>
public string UserName {get;}<br/>
when error will come ?<br/>
<br/>
<br/>
**IQ: Morgan Stanley: What types of binding present in VF:** <br/>
1. Data binding
2. Action binding
3. Component binding (rarely user, almost outdated) (see below code just for over view) (people are using Ltng components)


### 3. Extension Controllers :
- It gives the benefit of Standard as well as Custom Controllers.
- We canuse the fascility or ease that we get in Standard controller as well as we can get the flexibility provided by the customr controller.
- We can get all these benefits in one single page using the Controller Extension
- We cant use more than 1 object in Standard Controller,as well as we cant use more than 1 class in Custome controller. But using Controller Extension, we can go beyond these limitiations.
- Controller Extenstions are widely used in higher level Visual force page where we want to implement complex kind of logic n produce the related UI
<br/>
**Syntax:**<br/>

`
<apex:page standardController="Account" extension="Class_1, Class_2, Class_3"></apex:page>
`















