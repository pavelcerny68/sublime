# sublime
cs - jak nastavit terminus v sublime pro jazyk python

de - wie man in sublime für python terminus setzt

en - how to set a terminus in sublime for python

-----------------------------------------------------------------------
{
"target": "terminus_exec",
"cancel": "terminus_cancel_build",
"focus": true,
"cmd": ["python3", "-u", "$file"],
"file_regex": "^[ ]*File \"(...*?)\", line ([0-9]*)",
"selector": "source.python",

"env": {"PYTHONIOENCODING": "utf-8"},

"windows": {
    "cmd": ["py", "-u", "$file"],
},

"variants":
[
    {
        "name": "Syntax Check",
        "cmd": ["python3", "-m", "py_compile", "$file"],

        "windows": {
            "cmd": ["py", "-m", "py_compile", "$file"],
        }
    }
]
}
-----------------------------------------------------------------------
