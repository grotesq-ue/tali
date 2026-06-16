# **tali**
> **T**ool **A**ssemblage for **L**ocal **I**nference

This is just a scaffolding template for an opinionated local inference setup. Feel free to tweak and extend it to your liking.

## 🛠 **Setup** {#setup}

1. Install and setup **mise-en-place** package manager. See [mise-en-place installation guide](https://mise.jdx.dev/installing-mise.html).

2. Get the template:
```
mise exec node -- npx giget gh:grotesq-ue/tali local-inference
```

3. Change directory to the templated folder.
```
cd local-inference
```

4. Install the dependencies.
```
mise install
```

5. Run it.
```
task launch
```

> [!NOTE]
> Default models will be downloaded during the initial launch. This might take some time.

> [!TIP]
> Prepopulate `models/embedding` and `models/reasoning` with GGUF files to skip the download for the default models.

> [!TIP]
> Use [llmfit](https://www.llmfit.org/) to find out which models are compatible with your local machine.

6. Go to [http://localhost:8080/](http://localhost:8080/) and configure your local AI platform. See [Open WebUI Documentation](https://docs.openwebui.com/).

## 🗂 **Folder Structure**
```
📁 local-inference
  📁 .data
  📁 models
    📁 embedding
      🤖 <EMBEDDING_MODEL>.gguf
    📁 reasoning
      🤖 <REASONING_MODEL>.gguf
  🙈 .gitignore
  ⚙ cog.toml
  ⚙ lefthook.yml
  📜 LICENSE
  ⚙ mise.toml
  📖 README.md
  ⚙ Taskfile.yaml
```
