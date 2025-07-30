# 🔐 Multithreaded Hash Cracker in Python

A powerful and flexible tool for cracking hashed passwords using either a wordlist or brute-force approach. This Python-based utility supports multiple hash algorithms and uses multithreading to speed up the cracking process.

---

## 🚀 Features

- 🔄 **Supports Multiple Hashing Algorithms**:
  - `md5`, `sha1`, `sha224`, `sha256`, `sha384`, `sha512`
  - `sha3_224`, `sha3_256`, `sha3_384`, `sha3_512`
- 💡 **Two Cracking Modes**:
  - **Wordlist-based attack**: Use custom or popular wordlists like `rockyou.txt`.
  - **Brute-force attack**: Generates passwords from character sets and lengths you specify.
- ⚡ **Multithreaded Cracking**: Faster execution using Python's `ThreadPoolExecutor`.
- 📊 **Progress Visualization**: Real-time feedback using the `tqdm` progress bar.
- 🔧 **Customizable CLI Interface** via `argparse`.

---

## 🧪 How It Works

### 🔹 Wordlist Mode

The tool reads each password from the wordlist, hashes it, and compares it to the target hash.

```bash
python hash_cracker.py <HASH> -w wordlist.txt --hash_type md5
