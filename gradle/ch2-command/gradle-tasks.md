执行 `gradle init` 命令选择 application 类型后执行 `gradle tasks` 的结果如下：

```
$ gradle tasks

> Task :tasks

------------------------------------------------------------
Tasks runnable from root project
------------------------------------------------------------

Application tasks
-----------------
run - Runs this project as a JVM application

Build tasks
-----------
assemble - Assembles the outputs of this project.
build - Assembles and tests this project.
buildDependents - Assembles and tests this project and all projects that depend on it.
buildNeeded - Assembles and tests this project and all projects it depends on.
classes - Assembles main classes.
clean - Deletes the build directory.
jar - Assembles a jar archive containing the main classes.
testClasses - Assembles test classes.

Build Setup tasks
-----------------
init - Initializes a new Gradle build.
wrapper - Generates Gradle wrapper files.

Distribution tasks
------------------
assembleDist - Assembles the main distributions
distTar - Bundles the project as a distribution.
distZip - Bundles the project as a distribution.
installDist - Installs the project as a distribution as-is.

Documentation tasks
-------------------
javadoc - Generates Javadoc API documentation for the main source code.

Help tasks
----------
buildEnvironment - Displays all buildscript dependencies declared in root project 'type-application'.
components - Displays the components produced by root project 'type-application'. [incubating]
dependencies - Displays all dependencies declared in root project 'type-application'.
dependencyInsight - Displays the insight into a specific dependency in root project 'type-application'.
dependentComponents - Displays the dependent components of components in root project 'type-application'. [incubating]
help - Displays a help message.
kotlinDslAccessorsReport - Prints the Kotlin code for accessing the currently available project extensions and conventions.
model - Displays the configuration model of root project 'type-application'. [incubating]
projects - Displays the sub-projects of root project 'type-application'.
properties - Displays the properties of root project 'type-application'.
tasks - Displays the tasks runnable from root project 'type-application'.

Verification tasks
------------------
check - Runs all checks.
test - Runs the unit tests.

Rules
-----
Pattern: clean<TaskName>: Cleans the output files of a task.
Pattern: build<ConfigurationName>: Assembles the artifacts of a configuration.
Pattern: upload<ConfigurationName>: Assembles and uploads the artifacts belonging to a configuration.

To see all tasks and more detail, run gradle tasks --all

To see more detail about a task, run gradle help --task <task>

BUILD SUCCESSFUL in 21s
1 actionable task: 1 executed
```
