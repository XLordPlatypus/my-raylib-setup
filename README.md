# Raylib-Go setup

From here: https://github.com/gen2brain/raylib-go?tab=Zlib-1-ov-file

## Install Go
```bash
sudo pacman -S go
```

## Create Folder
```bash
mkdir project_folder
```

## Init Project
```bash
go mod init project_name
```

## Get Raylib
```bash
go get -v -u github.com/gen2brain/raylib-go/raylib
```

## Example
```go
package main

import rl "github.com/gen2brain/raylib-go/raylib"

func main() {
	rl.InitWindow(800, 450, "raylib [core] example - basic window")
	defer rl.CloseWindow()

	rl.SetTargetFPS(60)

	for !rl.WindowShouldClose() {
		rl.BeginDrawing()

		rl.ClearBackground(rl.RayWhite)
		rl.DrawText("Congrats! You created your first window!", 190, 200, 20, rl.LightGray)

		rl.EndDrawing()
	}
}
```

## Commands

```bash
go run main.go
```

```bash
go build main.go
```
