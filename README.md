# vaik-mnist-count-dataset

Create MNIST count dataset

## Example

![count_dataset_all](https://github.com/vaik-info/vaik-mnist-count-dataset/assets/116471878/24e8166c-a420-4edb-b8b3-4f2d311de01b)
![count_dataset](https://github.com/vaik-info/vaik-mnist-count-dataset/assets/116471878/44fc5c4a-90fc-4898-85b0-a573f6bdf816)

## Usage

``` shell
pip install -r requirements.txt
python main.py --output_dir_path ~/.vaik-mnist-count-dataset \
                --classes_txt_path ~/GitHub/vaik-mnist-count-dataset/classes.txt \
                --train_sample_num 40000 \
                --valid_sample_num 100 \
                --image_max_size 320 \
                --image_min_size 196 \
                --char_max_size 64 \
                --char_min_size 32 \
                --char_max_num 6 \
                --char_min_num 2
```

## Output

- classes.txt

```
zero
one
two
```


- classes.json

```
{
    "classes": [
        "zero",
        "one",
        "two"
    ]
}
```

- {image_base_name}.json

```json
{"two": 5, "one": 2, "zero": 2}
```

- raw image and json for train and validation

![count_dataset](https://github.com/vaik-info/vaik-mnist-count-dataset/assets/116471878/44fc5c4a-90fc-4898-85b0-a573f6bdf816)


