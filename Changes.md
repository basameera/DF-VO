# Change made to make it run

https://github.com/Huangying-Zhan/DF-VO

### Command

* Mono - `python run.py -d options/kitti/kitti_default_configuration.yml -c options/kitti/kitti_mono_sc_0.yml -s 00`
* Stereo - `python run.py -c options/kitti/kitti_stereo_0.yml -s 00`

### .yml file

* `kitti_default_configuration.yml`
```yaml
ext: png
```

* `vo_modules.py`
```python
line 963: img_data_dir = os.path.join(img_seq_dir, "image_0")
```