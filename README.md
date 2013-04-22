newsgator-lookout360-3.5
========================

NewsGator Social Sites Lookout360 implementation for 3.5

Layers is a plugin for [jQuery](http://jquery.com) that gives you the ability to apply layers of functionality to a given element. Right now the functionality is limited to events but later may expand.

## Features

## Usage

Default usage:

```js
<script src="javascripts/ngRibbonAutoLoader.min.js"></script>
<script type="text/javascript">
	var registerNgRibbon = {
	  cacheKey: "634934240492550038"
	  , ribbonOptions: { fixedPosition: true
	    , backgroundColor: '#8bbc1d'
	    , lookoutUrl: 'https://engage.newsgator.com/my/site/Lookout.aspx'
	    , contextUrl: "https://engage.newsgator.com"
	    , enablePost: true
	    , additionalLinks: {
	      "Engage": {
	        "target": "_blank",
	        "url": "https://engage.newsgator.com/my/site/Lookout.aspx"
	      },
	      "NewsGator": {
	        "target": "_blank",
	        "url": "http://www.newsgator.com"
	      }
	    }
	    , additionalLinksPosition: 3
	    , tileRefreshInterval: 120000
	    , tileContainerWidth: '400px'
	    , revealIframeWidthClass: 'w750'
	    , isExternal: true
	    , localOverrides: { "fr-fr": { title:"Recherche360", titleTooltip:"{0} Ouvert", postTooltip:"Publier sur Recherche" } }
	    , enablePlaceHolderOnBody: true
	    , defaultLocalization: { 
	      "en-us": { "loading":"Loading", "ribbonPromptAuth":"Authenticate with SocialSites", "ribbonPreventLoading":"Hide on this page" } 
	    }
	  }
	  , target: 'body'
	};
	ngRibbonAutoLoader.init(registerNgRibbon.cacheKey, registerNgRibbon.ribbonOptions, registerNgRibbon.target);
</script>
```