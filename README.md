# Python

Sub RunPythonScript()

Dim objShell As Object
Dim PythonExePath as String, PythonScriptPath As String 
ActiveWorkbook.Save
ChDir ActiveWorkbook.Path

    Set objShell = VBA.CreateObject("Wscript.Shell")
    
    'PythonExePath = """ Insert Path to Python EXE here """
    'PythonScriptPath = """ Insert Path to Python SCRIPT here """
    
    objShell.Run PythonExePath & PythonScriptPath

End Sub
