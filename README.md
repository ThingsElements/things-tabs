# things-taps

## 프로파일 컴포넌트

## Example:
```html
  <div>
    <things-ajax
      auto
      id="resource-meta"
      method="GET"
      resource-url="entities/Alarm/resource_columns"
      last-response="{{metaData}}">
    </things-ajax>

    <things-ajax
      auto
      resource-url="alarms/:id"
      resource-action="index"
      resource-id="1"
      last-response="{{detailViewData}}">
    </things-ajax>

    <things-resource-tabs
      search-meta
      meta-data="{{metaData}}"
      resource-type="Alarm"
      resource-url="alarms"
      resource="{{detailViewData}}"
      attachable
      prop-extensible>
    </things-resource-tabs>
  </div>
```

*****
</br></br>


## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install

## Playing With Your Element

If you wish to work on your element in isolation, we recommend that you use
[Polyserve](https://github.com/PolymerLabs/polyserve) to keep your element's
bower dependencies in line. You can install it via:

    npm install -g polymer-cli

And you can run it via:

    polymer serve

Once running, you can preview your element at
`http://localhost:8080/components/things-alarm/`, where `things-alarm` is the name of the directory containing it.
