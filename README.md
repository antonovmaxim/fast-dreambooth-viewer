[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/antonovmaxim/fast-dreambooth-viewer/blob/main/fast-dreambooth-viewer.ipynb)

# fast-dreambooth-viewer

This is a repository for running your stable diffusion models trained in https://colab.research.google.com/github/TheLastBen/fast-stable-diffusion/blob/main/fast-DreamBooth.ipynb and others.
This repository is an "abbreviation" in the [camenduru style](https://github.com/camenduru/stable-diffusion-webui-colab) of [this repository](https://colab.research.google.com/github/TheLastBen/fast-stable-diffusion/blob/main/fast_stable_diffusion_AUTOMATIC1111.ipynb).


<details>
<summary> It also helps if you get same error: </summary>
<code>
Traceback (most recent call last):
  File "launch.py", line 297, in <module>
    start()
  File "launch.py", line 291, in start
    webui.webui()
  File "/content/stable-diffusion-webui/webui.py", line 133, in webui
    initialize()
  File "/content/stable-diffusion-webui/webui.py", line 63, in initialize
    modules.sd_models.load_model()
  File "/content/stable-diffusion-webui/modules/sd_models.py", line 313, in load_model
    load_model_weights(sd_model, checkpoint_info)
  File "/content/stable-diffusion-webui/modules/sd_models.py", line 196, in load_model_weights
    sd = read_state_dict(checkpoint_file)
  File "/content/stable-diffusion-webui/modules/sd_models.py", line 173, in read_state_dict
    pl_sd = torch.load(checkpoint_file, map_location=map_location or shared.weight_load_location)
  File "/content/stable-diffusion-webui/modules/safe.py", line 106, in load
    return load_with_extra(filename, extra_handler=global_extra_handler, *args, **kwargs)
  File "/content/stable-diffusion-webui/modules/safe.py", line 151, in load_with_extra
    return unsafe_torch_load(filename, *args, **kwargs)
  File "/usr/local/lib/python3.8/dist-packages/torch/serialization.py", line 795, in load
    return _legacy_load(opened_file, map_location, pickle_module, **pickle_load_args)
  File "/usr/local/lib/python3.8/dist-packages/torch/serialization.py", line 1002, in _legacy_load
    magic_number = pickle_module.load(f, **pickle_load_args)
_pickle.UnpicklingError: invalid load key, '<'.
</code>
</details>

## Credits
[AUTOMATIC1111](https://github.com/AUTOMATIC1111)<br>
[camenduru](https://github.com/camenduru)<br>
[TheLastBen](https://github.com/TheLastBen)