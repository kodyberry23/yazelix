# Yazi-Helix File Tree v2: the sidebar can now be closed

Example with two or more panes open and sidebar open
![image](https://github.com/luccahuguet/yazi-files/assets/27565287/557eecbf-6eeb-48f9-8de4-252f78bda4fd)

Example with two or more panes open and sidebar closed
![image](https://github.com/luccahuguet/zellij-files/assets/27565287/4f63de6e-4df7-452f-9877-90461071b673)


This layout is called `stack_sidebar`!
Obs: it is already set in my config, but if you did not copy my config, you can set it with `default_layout "stack_sidebar"` in yours.

The base (starting) layout has 4 panes
![image](https://github.com/luccahuguet/zellij-files/assets/27565287/adc6162c-a1ec-4635-b217-aa7a9ba691c5)

- the tab-bar at the top
- the status-bar at the bottom
- a [yazi](https://yazi-rs.github.io/features) pane with 20% width acting as a side-bar, to the left
- and an empty pane to the right

After you create a fifth pane, you leave the base layout:
- You're now able to open and close the sidebar by switching swap layouts 
- You can add more swap layouts if you want
- The first two screenshots showcase the two layouts
- The fith pane, to the left, is the one where new panes will appear, stacked

### Improvements over v1: 
- now you can open and close the sidebar
- there is no nushell dependency anymore
- the layout kdl files are simpler than before

### Roadmap: I would like to 
- further simplify the kdl files, there is still some code repetion
- be able to open and close the sidebar with just 4 panes, currently that only works with 5 or more
- have a third swap layout that is a full yazi pane (showing parents and preview, [see more](https://github.com/luccahuguet/yazi-files))
- (for the item above to work, yazi would have to be able to recieve config as an argument)
  
### Other layout files in the repo: stack_sidebar_zjstatus (not the default)
- this is a cool layout that takes more configuration to work but enables a "more powerful tab-bar" that shows the time and the current layout for example, if you configure it to do it
- to enable it you have to change the config `default_layout "stack_sidebar_zjstatus"` and  install [zjstatus](https://github.com/dj95/zjstatus) placing the path in your layout kdl file
- basically, if you want to lose the status-bar, this more powerfull tab-bar can help out
