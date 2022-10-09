# Unittest doesn't work, fixed on User Settings
When i launch My Unit Test, I receive the error
```
was not able to get the file imported with "FROM" ("ModuleNotFoundError: No module named X")
```
So I fixed it by User Settings
1.CTRL + SHIFT + P
2. Choose User Setting
3.Add
```
{
    "terminal.integrated.env.windows": { "PYTHONPATH": "${workspaceFolder}" }
}
```
