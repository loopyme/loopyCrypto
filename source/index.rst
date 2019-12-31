

LoopyCryptor
^^^^^^^^^^^^

.. toctree::
   :maxdepth: 2
   :caption: Contents:



Examples
========
All functions are implemented in Class:Cryptor, but we use lambda functions to wrapped up the Cryptor functions. So you can use it easier. Like this:

.. code-block:: python

    import loopyCryptor

    # generate a pair of key
    public_key, private_key = loopyCryptor.generate_RSA_key()

    # encrypt
    text = "I hate verilog."
    cipher_byte = loopyCryptor.RSA_encrypt(text,public_key)

    # decrypt
    decrypt_text = loopyCryptor.RSA_decrypt(cipher_byte,private_key)
    print(decrypt_text) # I hate verilog.

API
===
.. automodule:: loopyCryptor.Cryptor.Cryptor
   :members: set_AES_key, generate_RSA_key, generate_AES_key, AES_encrypt, AES_decrypt, RSA_encrypt, RSA_decrypt

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`