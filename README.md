a = [
    ["floder", "coursework.doc", "floder", "pict.png", "data.accdb"],
    ["icon.ico", "script.js", "index.html", "style.css", "prog.py"],
    ["my_song.mp3", "anapa-2003.jpg", "cs 1.6.exe", "floder", "cheat.txt"],
    ["notes.txt", "main.py", "work.pdf", "cartoon.mp4", "array.py"],
    ["project.psd", "cycle.py", "floder", "cycle.js", "turtle.py"],
]
print("Исходный массив:")
for i in range(5):
    for j in range(5):
        print(a[i][j], end=" ")
    print()
    for i in range(5):
        for j in range(5):
            if a[i][j] == "floder":
                a[i][j] = "_"
                if a[i][j] == "data.accdb":
                    a[i][j] = "data.sq1"
print("\nПосле изменений:")
for i in range(5):
    for j in range(5):
        print(a[i][j], end=" ")
    print()
py_list = []
for i in range(5):
    for j in range(5):
        if ".py" in a[i][j]:
            py_list.append(a[i][j])
print("\nФайл с расширением .py:")
for i in range(len(py_list)):
    print(py_list[i])

js_list = []

for i in range(5):
    for j in range(5):
        if ".js" in a[i][j]:
            js_list.append("new_" + a[i][j])

print("\nФайлы с расширением .js (new_):")
for i in range(len(js_list)):
    print(js_list[i])
