
Intellisense feature is not working .. 

VSCode 1.71.2
Python: 3.7.10
'Intellicode' Extension: enabled


settings.json
{
"python.defaultInterpreterPath": "C:\\Users\\LENOVO\\AppData\\Local\\Microsoft\\WindowsApps\\python3.10.exe",
"terminal.integrated.profiles.windows": {
"PowerShell": {
"source": "PowerShell",
"icon": "terminal-powershell"
},
"Command Prompt": {
"path": [
"${env:windir}\\Sysnative\\cmd.exe",
"${env:windir}\\System32\\cmd.exe"
],
"args": [],
"icon": "terminal-cmd"
},
"Git Bash": {
"source": "Git Bash"
}
},
"window.autoDetectColorScheme": true,
"editor.quickSuggestions": {
"strings": "on"
},
"python.autoComplete.extraPaths": ["C:\\Users\\LENOVO\\AppData\\Local\\Packages\\PythonSoftwareFoundation.Python.3.10_qbz5n2kfra8p0\\LocalCache\\local-packages\\Python310"],
"python.analysis.extraPaths": ["C:\\Users\\LENOVO\\AppData\\Local\\Packages\\PythonSoftwareFoundation.Python.3.10_qbz5n2kfra8p0\\LocalCache\\local-packages\\Python310"],
"workbench.preferredDarkColorTheme": "Visual Studio Dark",
"vsintellicode.features.python.deepLearning": "enabled",
"vsintellicode.java.completionsEnabled": false,
"intellicodeApiExamples.loggingLevel": "WARN",
"python.experiments.enabled": false
}


Re-install vs code in
      C:\Users\username\AppData\Local\Programs\Microsoft VS Code
