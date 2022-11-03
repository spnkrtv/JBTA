# Inspect your code

IIntelliJ IDEA has a set of features for code inspections that helps you find and fix misspellings, potential bugs, and incorrect data input. You can run inspections for all files in a project or define desirable [scopes](https://www.jetbrains.com/help/idea/configuring-scopes-and-file-colors.html).

Each detected issue gets a [severity level](https://www.jetbrains.com/help/idea/configuring-inspection-severities.html) indicating its significance. IntelliJ IDEA has a set of predefined severity levels, but you can also configure your own by using [inspection profiles](https://www.jetbrains.com/help/idea/customizing-profiles.html).

The process of inspection consists of four sections:

1. [Setting up the inspections](#set-up-inspections)
2. [Analyzing a file](#analyze-a-file)
3. [Analyzing a project](#analyze-a-project)
4. [Cleaning up the code](#code-cleanup)

## Set up inspections
<ol>
<li>Click <b>IntelliJ IDEA</b> in the upper left corner, then go to <b>Preferences</b> or use the <code>⌘,</code> shortcut.</li>
<li>In the tree, find <b>Editor</b> and navigate to <b>Inspections</b>:
<br><br>
<img src="https://github.com/spnkrtv/JBTA/blob/main/1-preferences-1.png" width="500"></li>
<br><br>
<li>Pick a technology to configure inspections for and check the needed boxes:
<br><br>
<img src="https://github.com/spnkrtv/JBTA/blob/main/2-preferences-2.png" width="500"></li>
</ol>

## Analyze a file

IntelliJ IDEA automatically analyzes your code in the editor and highlights detected issues while writing the code.

<ol>
<li>If you have a syntax error, you will see a warning icon on the issue line. In the top right corner, you will see the widget with the numbers of detected issues of each severity:
<br><br>
<img src="https://github.com/spnkrtv/JBTA/blob/main/3-severity.png" width="500"></li>
<li>If you click on the widget, you can examine each issue in the <b>Problems tool</b>:
<br><br>
<img src="https://github.com/spnkrtv/JBTA/blob/main/4-problems.png" width="500">
<br>If you double-click on the message, you will see the highlighted line with the issue. You can also right-click and select <b>Jump to source</b> in the menu or use the <code>⌘↓</code> shortcut.</li>

<li>Click on the message and click the 💡 icon on the left toolbar. You can also use the warning icon on the issue line in the editor:
<br><br>
<img src="https://github.com/spnkrtv/JBTA/blob/main/5-quickfix.png" width="400"></li>
<li>Select one of the options on the menu and then resolve the error.</li>
</ol>

If automated inspecting doesn’t suit you, you can set up an inspection [manually](https://www.jetbrains.com/help/idea/running-inspections.html#run-inspections-manually) and get a report with the detected issues.

## Analyze a project

In IntelliJ IDEA, you can inspect your entire project for issues. Currently, it is possible only for Java projects. If you use some other languages along with Java, it might work incorrectly.
<ol> 
<li>To turn on the project-wide analysis, open the <b>Problems</b> tool. To do that, click <b>View</b> in the upper left corner. Hover on <b>Tool Windows</b> and select <b>Problems</b>. You can also use the <code>⌘6</code> shortcut.</li>
<li>Select the <b>Project Errors</b> tab and click the <img src="https://github.com/spnkrtv/JBTA/blob/main/6-icon.png" width="20"> icon on the left toolbar.
Running the analysis for the first time in the project takes longer than it will in the following inspections. Once the analysis is finished, you will see a list of all detected issues in the project:
<br><br>
<img src="https://github.com/spnkrtv/JBTA/blob/main/7-projerrors.png" width="400">
<br>Find the issue line in the editor by double-clicking on the message or right-clicking and selecting <b>Jump to source</b> in the menu or using the <code>⌘ ↓</code> shortcut.  
</li>
<li>Click on the warning icon on the issue line, select one of the options on the menu and then resolve the error.</li>
</ol>

## Code cleanup

If you don’t want to fix all detected issues one by one, you can run the Code Cleanup and apply quick fixes to to all issues at once.
<ol>
<li>Click <b>Code</b> on the top menu and select <b>Code Cleanup</b>.</li>
<li>In the <b>Specify Code Cleanup Scope</b> dialog, select a scope to apply:
<br><br>
<img src="https://github.com/spnkrtv/JBTA/blob/main/8-cleanup.png" width="400">
<br>The cleanup runs using the default inspection profile. If you want to use a custom one, select it from the dropdown list or click Configure to create a new profile.</li>
<li>Click <b>Analyze</b> to start the cleanup.</li>
</ol>

Code cleanup applies quick fixes to issues using the selected inspection profile. You can check the results on the **Problems tool** and export them to one of the available formats.
Note that you can set up performing the code cleanup in the [silent mode](https://www.jetbrains.com/help/idea/resolving-problems.html#silent-cleanup), cleanup before [committing to Git](https://www.jetbrains.com/help/idea/resolving-problems.html#quick-fix-before-commit), and cleanup [on save](https://www.jetbrains.com/help/idea/resolving-problems.html#clean-up-on-save).

## See also

[Configure inspection profiles](https://www.jetbrains.com/help/idea/customizing-profiles.html)<br>
[Run manual inspections](https://www.jetbrains.com/help/idea/running-inspections.html)<br>
[Create custom inspections](https://www.jetbrains.com/help/idea/creating-custom-inspections.html)<br>
[Change inspection severity](https://www.jetbrains.com/help/idea/configuring-inspection-severities.html)<br>
[Learn the Problems tool](https://www.jetbrains.com/help/idea/problems-tool-window.html)<br>
[Analyze duplicates](https://www.jetbrains.com/help/idea/analyzing-duplicates.html)
