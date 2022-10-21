# THINGS IN HERE

## GEMS

```
gem "sassc-rails"
```
- sassc for scss

## MODELS
- project has many tasks
- task belongs to projects
- task has a completed at patch

```
  resources :projects do
    resources :tasks do
      member do 
        patch :complete
      end
    end
  end

```

## OTHER
- used custom stylings
- added font awesome and google font via

```
<link href='http://fonts.googleapis.com/css?family=Lato:300,400,700' rel='stylesheet' type='text/css'>
<link href="//maxcdn.bootstrapcdn.com/font-awesome/4.2.0/css/font-awesome.min.css" rel="stylesheet">
```
