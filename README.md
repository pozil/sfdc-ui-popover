# Salesforce Lightning Popover Component (Deprecated)

<img src="screenshots/media-example.png" width="300" align="right"/>

**WARNING:** this component is deprectated.<br/>
It is replaced by official Winter '18 built-in components:
- [lightning:helptext](https://developer.salesforce.com/docs/atlas.en-us.lightning.meta/lightning/aura_compref_lightning_helptext.htm) for text only tooltips
- [lightning:overlayLibrary](https://developer.salesforce.com/docs/atlas.en-us.lightning.meta/lightning/ref_lightning_overlayLibrary.htm) for media tooltips

## About
This is a generic popover (tooltip) component built using Salesforce Lightning.<br/>
This component is built with [SLDS](https://www.lightningdesignsystem.com/) style and does not rely on third party libraries.

<b>Features</b>

The Lightning Popover component provides the following features:
- support for any kind of markup in popover dialog
- high performance thanks to a pure CSS implementation

## Install
Install the Lightning Popover component as a managed package by clicking on this button:

<a href="https://login.salesforce.com/packaging/installPackage.apexp?p0=04t0Y000000xSc3">
  <img src="gfx/btn-install.png" width="100" alt="Install">
</a>

## Documentation
Component is documented using the Aura documentation.
You can access it from this URL (replace the domain):
https://<b>&lt;YOUR_DOMAIN&gt;</b>.lightning.force.com/auradocs/reference.app#reference?descriptor=ui_popover:popover&defType=component

## Sample application
Paste the following code in a new Lightning Application to try it out:

``` xml
<aura:application extends="force:slds">
	<div class="slds-grid slds-grid--frame slds-grid--align-center slds-grid--vertical-align-center">
		
		<div>Note that&nbsp;
		    <ui_popover:popover>
			<aura:set attribute="popoverBody">
			    <h3 class="slds-section-title">The Popover Title</h3>
			    <p class="slds-m-bottom--x-small">Some textual description or <b>any</b> kind of markup including other components.</p>
			</aura:set>
			<a href="javascript:void(0);">hovering over this content (not necessarily a link) triggers the popover</a>
		    </ui_popover:popover>
	&nbsp;and it renders really nicely with SLDS.</div>
	
	</div>
</aura:application>
```

It will render like this:

<img src="screenshots/basic-example.png" width="75%"/>
