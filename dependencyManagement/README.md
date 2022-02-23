#  DependencyManagement Example

## Element details

## Project structure

This project is an example of element `dependencyManagement `

There is only one module.  Settings in `dependencyManagement` will partially overwrite the dependency information of true dependencies.  Note that if a dependency setting in `dependencyManagement` is not used in the dependency or their transitive dependencies, is should not be list in the final dependency list.

## Operation

You can scan the project under the main folder `dependencyManagement` Ground truth are shown below