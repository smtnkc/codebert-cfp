# CodeBERT SSM

*Predicting the Software Size and Effort from the Code Using Natural Language Processing*

<img src="https://raw.githubusercontent.com/smtnkc/codebert-ssm/main/workflow.png" alt="workflow" />


### COSMIC Size Measurement Parameters

```python
dataset = 'codesearchnet_auto.csv'
source = 'code'
target = 'cosmic_function_number'
num_labels = 4
batch_size = 64
epochs = 5
lr = 2e-5
```

### Event-based Size Measurement Parameters

```python
dataset = 'green_balance_functions.csv'
source = 'Code'
target = 'Interaction' or 'Communication' or 'Process' or 'Effort'
num_labels = 1
batch_size = 16
epochs = 4
lr = 1e-4 or 2e-5
```

### Test Results

| Metric                | Performance       |
|-----------------------|-------------------|
| COSMIC size           | ACC = 84.5%       |
| Interaction Event     | NMAE = 1.10       |
| Communication Event   | NMAE = 1.80       |
| Process Event         | NMAE = 0.09       |
| Total Event           | NMAE = 0.13       |
| Effort                | NMAE = 0.18       |
