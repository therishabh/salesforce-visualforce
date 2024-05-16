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
