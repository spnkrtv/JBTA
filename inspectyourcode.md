# Inspect your code

IIntelliJ IDEA has a set of features for code inspections that helps you find and fix misspellings, potential bugs, and incorrect data input data. You can run inspections for all files in a project or define desirable [scopes](https://www.jetbrains.com/help/idea/configuring-scopes-and-file-colors.html).

Each detected issue gets a [severity level](https://www.jetbrains.com/help/idea/configuring-inspection-severities.html) indicating its significance. IntelliJ IDEA has a set of predefined severity levels, but you can also configure your own by using [inspection profiles](https://www.jetbrains.com/help/idea/customizing-profiles.html).

## Set up inspections
<ol>
<li>Click <b>IntelliJ IDEA</b> in the upper left corner, then go to <b>Preferences</b> or use the <code>⌘,</code> shortcut.</li>
<li>In the tree, find <b>Editor</b> and navigate to <b>Inspections</b>:

<img src="https://github.com/spnkrtv/JBTA/blob/main/1-preferences-1.png" width="500"></li>

<li>Pick a technology to configure inspections for and check the needed boxes:

<img src="https://github.com/spnkrtv/JBTA/blob/main/2-preferences-2.png" width="500"></li>

</ol>

## Analyze a file

IntelliJ IDEA automatically analyzes your code in the editor and highlights detected issues while writing the code.

<ol>
<li>If you have a syntax error, you will see a warning icon on the issue line. In the top right corner, you will see the widget with the numbers of detected issues of each severity:

<img src="https://github.com/spnkrtv/JBTA/blob/main/3-severity.png" width="500"></li>

<li>If you click on the widget, you can examine each issue in the <b>Problems tool</b>:
<br><br>
<img src="https://github.com/spnkrtv/JBTA/blob/main/4-problems.png" width="500">
  
If you double-click on the message, you will see the highlighted line with the issue. You can also right-click and select <b>Jump to source</b> in the menu or use the <code>⌘↓</code> shortcut.</li>

<li>Click on the message and click the 💡 icon on the left toolbar. You can also use the warning icon on the issue line in the editor:

<img src="https://github.com/spnkrtv/JBTA/blob/main/5-quickfix.png" width="400"></li>

<li>Select one of the options on the menu and then resolve the error.</li>
</ol>

If automated inspecting doesn’t suit you, you can set up an inspection [manually](https://www.jetbrains.com/help/idea/running-inspections.html#run-inspections-manually) and get a report with the detected issues.

## Analyze a project

In IntelliJ IDEA, you can inspect your entire project for issues. Currently, it is possible only for Java projects. If you use some other languages along with Java, it might work incorrectly.
 
To turn on the project-wide analysis, open the **Problems** tool. To do that, click **View** in the upper left corner. Hover on **Tool Windows** and select **Problems**. You can also use the `⌘6` shortcut.
