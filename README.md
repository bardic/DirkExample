# Dirk Example

## Install

```bash
dagger install https://github.com/bardic/Dirk@0.1.0
```

## Implement 

```golang
type DirkExample struct{}

func (d *DirkExample) Build(src *dagger.Directory) *dagger.Directory {
	return dag.Dirk().Build(src)
}
```

## Customize 

Replace username and password in the `*_secrets.env` 
Replace `./License/unity_personal_license.ulf` with your license

## Run

```bash
dagger call build --src=. export --path=./builds
```
