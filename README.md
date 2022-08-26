# DoN AI Navigation Plugin for Unreal Engine 5
This plugin provides a 3D dynamic pathfinding system for use with Unreal Engine 4 & 5. This system was first developed for [DoN The Nature Game](http://www.drunkonnectar.com/) and the owner decided to make a plugin out of the navigation module as a gift to the Unreal community. He abandoned the project some years back and I started to collect various fixes and pull requests after I updated it to the current version.

The plugin is primarly designed for Flying AIs based in dynamic or procedural worlds, which need to solve complex pathfinding tasks and other behavior not covered by Unreal's native AI navigation system or maps, which are too complex to be solved by simple ray-tracing/sweeping heuristics or a waypoint system.

Where possible, I recommend that you use Unreal's native AI navigation or simpler navigation strategies; use this system when the more conventional strategies cannot solve your pathfinding usecases.

The plugin provides the following:
* Navigation Manager actor for configuring the system
* "Fly To" behavior tree node that can be readily dropped into your behavior trees
* Nodes for managing dynamic collision and pathfinding in your scene.
* A pathfinding API that advanced users can use for custom navigation queries from either Blueprints or C++

# Sample Project
There is still is an old [sample project](http://www.drunkonnectar.com/3d-pathfinding-ue4/) to quickly test the system and understand the different usecases it covers.

# Overviews and Tutorials
* [Article describing how to build the plugin from source and apply a basic use case](https://medium.com/anti-clickbait-coalition/3d-pathfinding-in-unreal-engine-9b04f58ca50c?source=friends_link&sk=aeb7269c3c85841f87bb7ca99658c176)
* [![Youtube video - Overview and Tutorial](http://www.drunkonnectar.com/wp-content/uploads/2016/03/ThumbnailWithYoutubeIcon.jpg)](https://www.youtube.com/watch?v=6Tr_K551zvI)

# Technical Overview
For a technical overview of the project, please visit this [link](http://www.drunkonnectar.com/3d-pathfinding-ue4/#TechnicalOverview)


# How to install 3rd Party Plugins from GitHub or Source Code

1:To get started make sure you have the Unreal Engine installed along with Visual Studio. Make sure that you also have Visual Studio set up for game development with C++.
2:Create a project within the Unreal Engine editor, then save and close the program.
3:Locate the directory of your newly created project. For example C:\Users\User\Unreal Engine\MyProject
4:Create a “Plugins” folder and place the source code into the new directory. For example C:\Users\User\Unreal Engine\MyProject\Plugins
5:Navigate back to the top level of your project and right-click on the .uproject file. Select Generate Visual Studio Project.
6:Reopen the project with the Unreal Engine editor and Navigate to Edit>Plugins and enable (if already enabled don’t worry) your new plugin.
