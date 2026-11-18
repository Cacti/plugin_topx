# plugin_topx for Cacti

TopX ranks data sources by average or peak values using Cacti’s native Data
Source Statistics, for example CPU usage or interface traffic. Its configured
source definitions also support arithmetic operations. Enable Data Source
Statistics and allow it to collect samples before using TopX.

## Versions and compatibility

This README describes the `master` source branch.

| Code | Plugin version | Minimum Cacti declared in `INFO` |
| --- | --- | --- |
| [Source branch](INFO) | 0.7 | 1.0.0 |
| [Published 0.7](https://github.com/Cacti/plugin_topx/releases/tag/0.7) | 0.6 | 1.0.0 |

Use the published release’s assets and tagged documentation when installing that
package. Branch code can include later changes, even when its version number
matches the release. Cacti’s own PHP and database requirements also apply.

The release tag and embedded plugin version differ; the table quotes the
metadata shipped in that tag.

Install this plugin in **`<cacti-root>/plugins/topx`**, using the directory
name `topx` rather than `plugin_topx`.

## Author
Petr Macek (petr.macek@kostax.cz)

## Screenshot
![topx_0 4](https://user-images.githubusercontent.com/26485719/33798513-1a7a4dba-dd1a-11e7-8ffe-f7f76c5124ba.png)

## Installation
Copy directory topx to plugins directory  
Check file permission (Linux/unix - readable for www server)  
Enable plugin (Console -> Plugin management)   
    
## Upgrade    
Copy and rewrite files  
Check file permission (Linux/unix - readable for www server)  
Disable and deinstall old version (Console -> Plugin management)   
Install and enable new version (Console -> Plugin management)   
    
## Possible Bugs or any ideas?
If you find a problem, let me know via github or https://forums.cacti.net/viewtopic.php?f=5&t=56129
   

## Changelog
	--- 0.7
		Limit display graph for more than 50 records
		Add sort by peak
		
	--- 0.6
		Add arithmetical operation again
		Bug fix
		Graph display optimalization
		
	--- 0.5
		Add theme support
		Remove my data source poller code, using native dsstats
		Remove arithmetical operation (dsstats doesn't support this)
		 
 	--- 0.4
		Add chartJS graphs
		Add human readable values 
		Fix empty source

	--- 0.3
		rewrite for cacti 1.x

	--- 0.2
		Fixed error - logging too much
	
	--- 0.1
		Beginning


