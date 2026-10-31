# Deviating-Machine
A machine that deviates from the line of reasoning.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Can you deviate from that line, machine?" \
  | uvx deviating-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install deviating-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
deviating-machine -a multilogue.txt
```
Or:
```bash
deviating-machine multilogue.txt > response.txt
```
Or:
```bash
deviating-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import deviating_machine
```
