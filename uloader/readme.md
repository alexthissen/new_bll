# Micro Loader

This is a minimal loader for card files.

* ml.enc

  Encrypted header for 256K carts. Must be concatenated with the binary of the game.
  First byte of the game must contain the number of pages. Game goes to $200.

* ml512.enc

  Encrypted header for 512K carts. Must be concatenated with the binary of the game.
  First byte of the game must contain the number of pages. Game goes to $200.

* bll.enc

  Encrypted header for files with BLL header. Concatenate with a BLL file to build a ROM image.

* micro_loader.s

  Source of the loader.

* bll_loader.s

  Source of the loader.

* allff.lyx.bz2

  A binary with 256K $FF to fill the ROM file (better for flashing).

* demo.s

 A small demo doing nothing but showing the use of the CART_HEADER macro to build a ready to run LNX file from single source.