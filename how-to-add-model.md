## How to add models to mastml

1. Go to `MASTMLInitializer.py` and add another if-block to the `get_machinelearning_model`
   method, under either `regression` or `classifier` depending on your model.
2. In the same file, go to the `_models_and_tests_to_run` method and add a line for your model on
    the `self.configtemplate['Models and Tests to Run']['models'] = ...` line.
3. Copy and modify `example_input.conf` and do a test run of your model with `python ../MASTML.py myexample.conf`
