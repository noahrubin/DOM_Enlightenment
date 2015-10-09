Chapter 1: Node Overview
---
1.1: DOM is a hierarchy of JS node objects
	- Browser parses HTML into DOM tree, which is hierarchical representation
	- Made as API for XML documents but was then extended to HTML as API for languages like JavaScript
---
1.2: Node Object Types
	Most Common Node Types:
	- DOCUMENT_NODE (window.document)
	- ELEMENT_NODE (<body>, <a>, <p>, <script>, etc)
	- ATTRIBUTE_NODE (class="thisCLass")
	- TEXT_NODE (text chars including carriage return and white space)
	- DOCUMENT_FRAGMENT_NODE (document.createDocumentFragment() -- is a contianer for dom nodes that, when attached to DOM is replaced by children)
	- DOCUMENT_TYPE_NODE (<!DOCTYPE html>)
	--> these enums map to certain type of node object
	All Node Types:
	- ELEMENT_NODE  = 1
	- ATTRIBUTE_NODE  = 2
	- TEXT_NODE  = 3
	- CDATA_SECTION_NODE  = 4
	- ENTITY_REFERENCE_NODE  = 5
	- ENTITY_NODE  = 6
	- PROCESSING_INSTRUCTION_NODE  = 7
	- COMMENT_NODE  = 8
	- DOCUMENT_NODE  = 9
	- DOCUMENT_TYPE_NODE  = 10
	- DOCUMENT_FRAGMENT_NODE  = 11
	- NOTATION_NODE  = 12
	- DOCUMENT_POSITION_DISCONNECTED  = 1
	- DOCUMENT_POSITION_PRECEDING  = 2
	- DOCUMENT_POSITION_FOLLOWING  = 4
	- DOCUMENT_POSITION_CONTAINS  = 8
	- DOCUMENT_POSITION_CONTAINED_BY  = 16
	- DOCUMENT_POSITION_IMPLEMENTATION_SPECIFIC  = 32
	--> ATTRIBUTE_NODE is not actually part of tree, is historical (depreceated in DOM 4)
---
1.3: Sub-Node Objects and Inheritance
	- Each different node type extends Object > Node > *
	--> Inheritance chain can be long, e.g. Object > Node > Element > HTMLElement..
---
1.4: Properties and Methods of Working Nodes
	Node Properties:
		- childNodes
		- firstChild
		- lastChild
		- nextSibling
		- nodeName
		- nodeType
		- nodeValue
		- parentNode
		- previousSibling
	Node Methods:
		- appendChild()
		- cloneNode()
		- compareDocumentPosition()
		- contains()
		- hasChildNodes()
		- insertBefore()
		- isEqualNode()
		- removeChild()
		- replaceChild()
	Document Methods:
		- document.createElement()
		- document.createTextNode()
	HTML* Element Properties:
		- innerHTML
		- outerHTML
		- textContent
		- innerText
		- outerText
		- firstElementChild
		- lastElementChild
		- nextElementChild
		- previousElementChild
		- children
	HTML Element Methods:
		- insertAdjacentHTML()
---
1.5 Identifying the Type and Name of a Node
