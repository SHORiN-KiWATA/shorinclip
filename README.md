# shorinclip

My first bash script.

A wayland clipboard TUI based on `fzf` `wl-clipboad` `cliphist`. Using `kitty icat` for image preview and `ffmpegthumbnailer` for video thumb.

- installation

    ```
    yay -S shorinclip
    ```

- useage

    Manually run this command:
  
    ```
    wl-paste --watch cliphist store
    ```


    Then it just work. Also setup autostart in your wayland compositor's config file.


    For image preview, you need to install a terminal which supports `kitty icat` such as `kitty` or `ghostty`.

