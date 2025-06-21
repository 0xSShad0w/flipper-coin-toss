cmake_minimum_required(VERSION 3.13)\n\nproject(coin_toss_simple C)\n\nfind_package(Furi REQUIRED)\n\nadd_flipper_app(\n    coin_toss_simple\n    coin_toss.c\n)
