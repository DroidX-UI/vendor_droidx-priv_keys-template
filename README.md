
A cool template to sign DroidX-UI builds with `dev-keys`.

## Usage

1. Clone the repository 

```
git clone https://github.com/DroidX-UI/vendor_droidx-priv_keys-template.git vendor/droidx-priv/keys 
```

2. Go to the key directory 

```
cd vendor/droidx-priv/keys
```

3. Run the script

```
./gen_keys
```

It will generate the certificates in vendor/droidx-priv/keys and the actual keys used to generate the certificates in ~/.android-certs/.

It will also generate the makefiles based on the keys defined in the _data/ folder.

Backup AT ALL COSTS your ~/.android-certs/ and vendor/droidx-priv/keys folders AND NEVER LEAK THOSE. Losing these keys could prevent you from updating your DroidX-UI builds with the same keys, so formatting data would be required. Leakage of these keys can compromise the security and authenticity of your builds, requiring a new pair of keys to be generated.