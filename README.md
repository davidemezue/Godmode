# Godmode

## Lab Objective
Create the “God Mode” shell folder and use it to locate and open key Windows administration tools.

## Lab Purpose
“God Mode” is a nickname for a special Windows folder that lists most Control Panel and administration settings in one place, grouped by category.

It does not give you extra permissions or unlock hidden features. It is a convenient shortcut hub, and it is useful for IT administrators and technicians who need quick access to many tools.

## Lab Tool
- Windows 10 or Windows 11

## Lab Topology
Use a virtual PC or your own PC.

## Lab Walkthrough

### Task 1: Create a new folder

1. Right-click an empty area of the desktop.
2. Select New > Folder.

### Task 2: Turn the folder into the God Mode folder

Rename the folder to exactly:

```text
GodMode.{ED7BA470-8E54-465E-825C-99712043E01C}
```

Include the period and the curly brackets.

Press Enter.

The text before the period (GodMode) disappears, and the folder is now shown with a Control Panel-style icon and no visible name. This is expected.

**Tip:** You can use any name before the period (for example, `Admin Tools.{ED7BA470-8E54-465E-825C-99712043E01C}`) and that name will stay visible. Only the code after the period matters.

### Task 3: Explore the available settings

1. Double-click the new icon to open it.
2. Scroll through the list and note the categories, such as Administrative Tools, Device Manager, Network and Sharing Center, Power Options, Programs and Features, and Security and Maintenance.
3. Right-click inside the folder and use View > Details to make the list easier to read.

### Task 4: Open key tools from God Mode

Use the folder (or the search box in its window) to find and open each tool below. Record which category each one is listed under.

- Device Manager
- Power Options
- Programs and Features

Close each window after opening it.

### Task 5: Compare with Control Panel

1. Open Control Panel (search for it in the Start menu).
2. Find the same three tools there.

Compare:

- Device Manage (godmode | Control Panel)
- Power Options (godmode | Control Panel)
- Programs and Features (godmode | Control Panel)

**Answer:** Does God Mode give you any tools that Control Panel does not? Does it grant extra permissions?

**Expected finding:** It is the same set of tools in a single list, with no extra permissions.

### Task 6: Clean up

1. Close the God Mode folder.
2. Right-click the folder and select Delete. This is safe and leaves nothing behind.

## Troubleshooting

**The folder stays a normal folder:**

Check for typos, a missing period, or missing curly brackets. Make sure there is no extra space or hidden file extension in the name.

**You can't rename it:**

Make sure you are on the desktop or in a folder you have permission to edit.

## Notes

God Mode does not bypass security or administrator rights. Some tools will still ask for administrator approval.

Microsoft is gradually moving settings into the Settings app, so a few items may open Settings instead of the classic Control Panel.

### Command-line alternative

In Command Prompt, run:

```cmd
mkdir "%userprofile%\Desktop\GodMode.{ED7BA470-8E54-465E-825C-99712043E01C}"
```

## Conclusion

This lab explores the Windows God Mode shell folder, demonstrating how it centralizes access to administration tools and Control Panel settings without granting additional privileges.
