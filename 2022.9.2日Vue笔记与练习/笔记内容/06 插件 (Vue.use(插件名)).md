1. 首先我们需要创建一个js文件 放置插件

    **~~plugins.js~~**

    ```vue
    export default{
    	install(){
    		Vue.fillter()	插件1
    		插件2
    		插件3
    		插件4...
    		都是定义的全局功能
    	}
    }
    ```

    **~~引入插件 进行使用~~**

    在App.vue中 进行use引入

    ```vue
    import plugins from './plugins'
    Vue.use(plugins)
    ```

    