# Rumah Kita Sendiri (Home-Manager) with Nix Flakes.

> Lihat Video disini -> https://youtu.be/M2kyVx-DZAk 

## Prasyarat (Prerequisite)
* Nix: sudah dipasang di-komputer kamu
* Aktifkan "flakes"

## Perintah (Command)

### Build 

#### With nix build command

```console
# nix build .#homeConfigurations.<USER_IN_SET_ATTRIBUTES>.activationPackage
nix build .#homeConfigurations.rin.activationPackage
```

#### With home-manager command

```console
# home-manager build .#<USER_IN_SET_ATTRIBUTES>
home-manager build .#rin
```

### Switch

#### With activate command from ./result

```console
./result/activate
```

#### With home-manager command

```console
home-manager switch --flake .#rin
```

Thanks
