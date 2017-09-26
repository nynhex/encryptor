#### Basic Rails encryption

* Put these classes in `app/models` or `lib`
* Set a key by whatever method you like, but I recommend `rails secrets` or `SecureRandom.random_bytes(32)`
* In your model where you want to encrypt/decrypt simply call `serialize :your_attribute, Encryptor.new`
* Watch the magic
