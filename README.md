# Usage

*modify in 2024/08/21 tested on python3.10 with refcoco*

1. Download coco2014 train datasets from :https://cocodataset.org/#download (about 13 GB) and extract into `refer/data/images/mscoco/images/train2014`

2. clone this repositories https://github.com/cocodataset/cocoapi and following instruction to compile Pythonapi.

3. Download refcoco here 

   ```html
   https://web.archive.org/web/20220413011718/https://bvisionweb1.cs.unc.edu/licheng/referit/data/refcoco.zip
   ```

   and extract into `refer/data`

4. install following package:

   ```bash
   pip install scikit-image
   ```

5. Run `make` before using the code. It will generate `_mask.c` and `_mask.so` in `external/` folder.  If anything goes wrong , just use `pip install xxx` to install the missing package.

6. Modify `refer.py` line 336, change data_root into your absolute path.

7. Run `python3 refer.py`
