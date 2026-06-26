[Uploading frames_2026-06-26_20.13.54.pdf…]()
# Nav2_config
for fastlio_localization tf
[frames_2026-05-14_19.04.16.pdf](https://github.com/user-attachments/files/27755263/frames_2026-05-14_19.04.16.pdf)

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1b55fe21-c71b-4fdf-b34c-911fb6629b23" />

<img width="1589" height="913" alt="스크린샷 2026-05-17 18-28-49" src="https://github.com/user-attachments/assets/e9d312a0-0e14-4a95-80c9-d943b397d765" />

This is a revision of nav2 yaml in ros2 for fastlio-localization. The modification should also be made in nav2 because the odom is omitted in the tf in the fastlio revision.
Files in the system folder cannot be modified, so I copy them to my workspace or folder to modify them.
At this time, you need to write down the yaml location when executing the code.

```
ros2 launch nav2_bringup bringup_launch.py \
    use_sim_time:=false \
    autostart:=true \
    map:=/home/your/project//map.yaml \
    params_file:=/home/your_name/nav2_config/my_nav2_params.yaml
```
