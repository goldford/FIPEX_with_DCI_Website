
#FIPEX with the DCI 2020 Homepage
## Welcome! 

You've landed on the homepage for the Fish Passage Extension (FIPEX) with Dendritic Connectivity Index (DCI) project. 

The extensive fragmentation of river systems due to damming, road construction, and other development is a problem that many governments, academic institutions, communities, corporations, and environmental groups are trying to solve.  On the path to recovery of _longitudinal_ _connectivity_ (i.e., connectivity from headwaters to ocean / outflow) of river systems many questions arise, including:  

* How fragmented is a river system?
* How much of the fragmentation is due to anthropogenic barriers?
* How much does each barrier contribute to local fragmentation? 
* How much does each barrier contribute to system-wide fragmentation?
* How much habitat or proportion of the river will be restored or reconnected by a given project?
* What kind of habitat will be made available?
* How can limited funds be used most effectively?

River systems present unique challenges when attempting to assess the impacts of barriers and costs/benefits of habitat restoration and connectivity projects, making answering the above questions difficult, time consuming, or both. The Fish Passage Extension (FIPEX) with Dendritic Connectivity Index (DCI) is designed to help address these challenging questions. 

![FIPEX-DCI link](./assets/images/FIPEX_DCI_link.png)

The toolset is designed as an integrated 'Add-in' to the Geographic Information System (GIS) software ArcGIS Desktop™ (ArcMap™ 10.4+) by ESRI™.  It provides basic and advanced tools for assessing river systems with respect to their longitudinal connectivity and can assess individual and cumulative impacts of barriers to fish passage such as dams, weirs, and culverts.  FIPEX can be differentiated from other toolsets for river / watershed network analysis in that it leverages the geometric network model provided with the ESRI ArcGIS Desktop™ suite. 

![network model image](./assets/images/network_flow.png)

By using the geometric network model, the direction of flow can be set and network analyses can be conducted without the need for Digital Elevation Models, careful attention to digitization direction, or other datasets; users simply need river lines  and a river outflow point. 

FIPEX is made freely available courtesy of various developers and sponsoring institutions over the years. 

#FIPEX Overview
[back to top](#fipex-with-the-dci-2020-homepage)

The Fish Passage Extension for ArcGIS 10.4 (FIPEX) with the Dendritic Connectivity Index (DCI) is a toolset for assessing the individual and cumulative effects of watercourse obstacles on the connectivity of river systems. FIPEX offers the ability to quantitatively assess the effects of real or anticipated barriers.  

[Gabby's Video]

The following are the main features:   
1.	Summarize river quantity affected by one or many barriers, where habitat affected may be defined as: 

	a)	habitat immediately upstream of a barrier (until the next barrier or headwaters)
	
	b)	habitat immediately downstream of a barrier (until the next barrier or headwaters)
	
	c)	total habitat upstream of a barrier (ignoring all other barriers)
	
	d)	total habitat downstream of a barrier (with the flow of the system, until the ocean / sink)

	e)	total habitat downstream of a barrier (ignoring flow direction)
2.	Allow flexible definition of habitat quantity, allowing users to choose from: 
	
	a)	Length / linear network (e.g., metres)
	
	b)	Polygonal / area network (e.g., hectares) 
	
	c)	Either (a) or (b) while excluding certain features (e.g., stillwater, wetland, lake 'spines')
3.	Classify river and assess quantity by class (e.g., lakes, river, wetland, urban area). 
4.	Exclude certain barriers (e.g., waterfalls) from analyses.
5.	Calculate the Dendritic Connectivity Index (DCI): 
	
	a)	DCId where d stands for ‘diadromous’ connectivity; assessing connectivity from sources to sink. 
	
	b)	DCIp where p stands for ‘potamodromous’ connectivity; assessing connectivity within the system ignoring flow direction (i.e., undirected connectivity)
6.	Assess the ‘sectional’ DCI for each barrier; evaluate the impact of individual barriers on directed connectivity with attention to natural vs artificial barriers.


# Who is the Typical User of FIPEX?

Ultimately, the goal of FIPEX is to provide the everyday user with a decision support tool for fish passage and riverine connectivity assessment.  Setup of FIPEX 10.4 is best done by an intermediate to advanced user of ArcGIS™ - typically a GIS technician or GIS specialist. Familiarity with the geometric network model (usage of the Utility Network Analyst toolbar) is an asset. 

After a river network is created, barriers are organized and labelled, quality assurance on the data is done, FIPEX is installed, options are set, and preliminary tests are done, FIPEX can be used as a decision support tool by people without GIS skills. The flexibility offered by the toolset and advanced options such as coupling with the statistical software, 'R', mean that the typical user should have experience with ArcGIS and technical knowledge of windows-based software and operating systems.  


# The Dendritic Connectivity Index (DCI)

The Dendritic Connectivity Index (DCI) is a measure of longitudinal connectivity of a river system (Cote et al., 2009). 

![network-model](./assets/images/cote2009figure.png)
Cote, D., Kehler, D. G., Bourne, C., & Wiersma, Y. F. (2009). A new measure of longitudinal connectivity for stream networks. Landscape Ecology, 24(1), 101-113.

The framework calculates the expected connectivity of a river system given the barriers present, barrier passability, barrier type, habitat quantity and river length. The DCI comes in several ‘flavours’: 
* __DCI__ __diadromous__ __(DCId)__: connectivity to / from the sink or outflow
* __DCI__ __potamodromous__ __(DCIp)__: connectivity to / from every river segment to every other river segment
* __DCI__ __sectional__ __(DCIs)__: connectivity to / from a given segment
* __DCI__ __(natural-only)__: connectivity considering only natural barriers
* __DCI__ __with__ __distance__ __decay__: connectivity considering maximum distance threshold or distance decay function (can be applied to any of the DCI ‘flavours’ above)



You can use the [editor on GitHub](https://github.com/goldford/FIPEX_with_DCI_Website/edit/master/README.md) to maintain and preview the content for your website in Markdown files.


Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/goldford/FIPEX_with_DCI_Website/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
