1. Clone this repo
```
git clone https://github.com/PatrickAlphaC/web3_py_simple_storage
cd web3_py_simple_storage
```
2. Setup a [local ganache chain](https://www.trufflesuite.com/ganache)
3. Install requirements
```bash
pip install -r requirements.txt
```
4. Set your private keys and address, and adjust this section appropriately:
```python
# For connecting to ganache
w3 = Web3(Web3.HTTPProvider("http://0.0.0.0:8545"))
chaind_id = 1337
my_address = "0x94B806BB0e455576ea46193D9DBbB08d1cc57Da9"
private_key = os.getenv("PRIVATE_KEY")
```
To set your private key as an environment variable, run `export PRIVATE_KEY=0xasdfasdfasfdasf`. If you're confused on how environment variables work, just set:
```python
private_key = "0xYOUR_KEY_HERE"
```
5. Run 
```
python deploy.py
```

To run on a testnet, just change these variables to whatever testnet you want to work with:
```
w3 = Web3(Web3.HTTPProvider("http://0.0.0.0:8545"))
chaind_id = 1337
my_address = "0x94B806BB0e455576ea46193D9DBbB08d1cc57Da9"
private_key = os.getenv("PRIVATE_KEY")
```
And make sure you have testnet ETH for whatever testnet you're on!
