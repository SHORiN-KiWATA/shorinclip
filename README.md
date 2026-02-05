# shorinclip

My first bash script.

A wayland clipboard TUI based on `fzf` `wl-clipboad` `cliphist`. Use `kitty icat` for image preview and `ffmpegthumbnailer` for video thumb generation.

- some image

    ![](pictures/showcase1.png)

    ![](pictures/showcase2.png)

- installation

    ```
    yay -S shorinclip
    ```
    For image preview, a terminal which supports `kitty icat` is needed, such as `kitty` or `ghostty`.

- useage

    Open cliphist daemon with this command:
  
    ```
    wl-paste --watch cliphist store
    ```
    
    Open tui with command: `shorinclip` 

    Then it just works. Also setup autostart in your wayland compositor's config file.

    - Niri

        ```
        spawn-at-startup "wl-paste" "--watch" "cliphist" "store"
        ```

    - Hyprland

        ```
        exec-once = wl-paste --watch cliphist store
        ```

