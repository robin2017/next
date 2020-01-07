{"title":"custom event value","meta":{"title":"custom event value","description":"\n<p>custom <code>value</code> by api <code>getValueFromEvent</code></p>\n","order":"2"},"codes":{"jsx":"import { Button, Input, Field } from '@alifd/next';\n\n\nclass App extends React.Component {\n\n    field = new Field(this);\n\n    normFile(list) {\n        if (Array.isArray(list)) {\n            return list;\n        }\n        return list && list.fileList;\n    }\n\n    normDate(date, strdate) {\n        console.log('normDate:', date, strdate);\n        return strdate;\n    }\n\n    render() {\n        const init = this.field.init;\n\n        return (<div>\n            <Input {...init('name', { getValueFromEvent: (value) => {\n                if (value.match(/##/)) {\n                    return value;\n                } else {\n                    return `## title-${value}`;\n                }\n            }})} />\n            <Button type=\"primary\" onClick={() => {\n                console.log(this.field.getValues());\n            }}>getValues</Button>\n        </div>);\n    }\n}\n\n\nReactDOM.render(<App/>, mountNode);\n"},"body":"\n````jsx\nimport { Button, Input, Field } from '@alifd/next';\n\n\nclass App extends React.Component {\n\n    field = new Field(this);\n\n    normFile(list) {\n        if (Array.isArray(list)) {\n            return list;\n        }\n        return list && list.fileList;\n    }\n\n    normDate(date, strdate) {\n        console.log('normDate:', date, strdate);\n        return strdate;\n    }\n\n    render() {\n        const init = this.field.init;\n\n        return (<div>\n            <Input {...init('name', { getValueFromEvent: (value) => {\n                if (value.match(/##/)) {\n                    return value;\n                } else {\n                    return `## title-${value}`;\n                }\n            }})} />\n            <Button type=\"primary\" onClick={() => {\n                console.log(this.field.getValues());\n            }}>getValues</Button>\n        </div>);\n    }\n}\n\n\nReactDOM.render(<App/>, mountNode);\n````","html":"<script>(function(){'use strict';\n\nvar _createClass = function () { function defineProperties(target, props) { for (var i = 0; i < props.length; i++) { var descriptor = props[i]; descriptor.enumerable = descriptor.enumerable || false; descriptor.configurable = true; if (\"value\" in descriptor) descriptor.writable = true; Object.defineProperty(target, descriptor.key, descriptor); } } return function (Constructor, protoProps, staticProps) { if (protoProps) defineProperties(Constructor.prototype, protoProps); if (staticProps) defineProperties(Constructor, staticProps); return Constructor; }; }();\n\nvar _next = require('@alifd/next');\n\nfunction _classCallCheck(instance, Constructor) { if (!(instance instanceof Constructor)) { throw new TypeError(\"Cannot call a class as a function\"); } }\n\nfunction _possibleConstructorReturn(self, call) { if (!self) { throw new ReferenceError(\"this hasn't been initialised - super() hasn't been called\"); } return call && (typeof call === \"object\" || typeof call === \"function\") ? call : self; }\n\nfunction _inherits(subClass, superClass) { if (typeof superClass !== \"function\" && superClass !== null) { throw new TypeError(\"Super expression must either be null or a function, not \" + typeof superClass); } subClass.prototype = Object.create(superClass && superClass.prototype, { constructor: { value: subClass, enumerable: false, writable: true, configurable: true } }); if (superClass) Object.setPrototypeOf ? Object.setPrototypeOf(subClass, superClass) : subClass.__proto__ = superClass; }\n\nvar App = function (_React$Component) {\n    _inherits(App, _React$Component);\n\n    function App() {\n        var _ref;\n\n        var _temp, _this, _ret;\n\n        _classCallCheck(this, App);\n\n        for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {\n            args[_key] = arguments[_key];\n        }\n\n        return _ret = (_temp = (_this = _possibleConstructorReturn(this, (_ref = App.__proto__ || Object.getPrototypeOf(App)).call.apply(_ref, [this].concat(args))), _this), _this.field = new _next.Field(_this), _temp), _possibleConstructorReturn(_this, _ret);\n    }\n\n    _createClass(App, [{\n        key: 'normFile',\n        value: function normFile(list) {\n            if (Array.isArray(list)) {\n                return list;\n            }\n            return list && list.fileList;\n        }\n    }, {\n        key: 'normDate',\n        value: function normDate(date, strdate) {\n            console.log('normDate:', date, strdate);\n            return strdate;\n        }\n    }, {\n        key: 'render',\n        value: function render() {\n            var _this2 = this;\n\n            var init = this.field.init;\n\n            return React.createElement(\n                'div',\n                null,\n                React.createElement(_next.Input, init('name', { getValueFromEvent: function getValueFromEvent(value) {\n                        if (value.match(/##/)) {\n                            return value;\n                        } else {\n                            return '## title-' + value;\n                        }\n                    } })),\n                React.createElement(\n                    _next.Button,\n                    { type: 'primary', onClick: function onClick() {\n                            console.log(_this2.field.getValues());\n                        } },\n                    'getValues'\n                )\n            );\n        }\n    }]);\n\n    return App;\n}(React.Component);\n\nReactDOM.render(React.createElement(App, null), mountNode);})()</script><div class=\"highlight\"><pre class=\"language-jsx\"><code class=\"language-jsx\"><span class=\"token keyword\">import</span> <span class=\"token punctuation\">{</span> Button<span class=\"token punctuation\">,</span> Input<span class=\"token punctuation\">,</span> Field <span class=\"token punctuation\">}</span> <span class=\"token keyword\">from</span> <span class=\"token string\">'@alifd/next'</span><span class=\"token punctuation\">;</span>\n\n\n<span class=\"token keyword\">class</span> <span class=\"token class-name\">App</span> <span class=\"token keyword\">extends</span> <span class=\"token class-name\">React<span class=\"token punctuation\">.</span>Component</span> <span class=\"token punctuation\">{</span>\n\n    field <span class=\"token operator\">=</span> <span class=\"token keyword\">new</span> <span class=\"token class-name\">Field</span><span class=\"token punctuation\">(</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n\n    <span class=\"token function\">normFile</span><span class=\"token punctuation\">(</span><span class=\"token parameter\">list</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n        <span class=\"token keyword\">if</span> <span class=\"token punctuation\">(</span>Array<span class=\"token punctuation\">.</span><span class=\"token function\">isArray</span><span class=\"token punctuation\">(</span>list<span class=\"token punctuation\">)</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n            <span class=\"token keyword\">return</span> list<span class=\"token punctuation\">;</span>\n        <span class=\"token punctuation\">}</span>\n        <span class=\"token keyword\">return</span> list <span class=\"token operator\">&amp;&amp;</span> list<span class=\"token punctuation\">.</span>fileList<span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n\n    <span class=\"token function\">normDate</span><span class=\"token punctuation\">(</span><span class=\"token parameter\">date<span class=\"token punctuation\">,</span> strdate</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n        console<span class=\"token punctuation\">.</span><span class=\"token function\">log</span><span class=\"token punctuation\">(</span><span class=\"token string\">'normDate:'</span><span class=\"token punctuation\">,</span> date<span class=\"token punctuation\">,</span> strdate<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n        <span class=\"token keyword\">return</span> strdate<span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n\n    <span class=\"token function\">render</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n        <span class=\"token keyword\">const</span> init <span class=\"token operator\">=</span> <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>field<span class=\"token punctuation\">.</span>init<span class=\"token punctuation\">;</span>\n\n        <span class=\"token keyword\">return</span> <span class=\"token punctuation\">(</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>div</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n            &lt;Input </span><span class=\"token punctuation\">{</span><span class=\"token operator\">...</span><span class=\"token function\">init</span><span class=\"token punctuation\">(</span><span class=\"token string\">'name'</span><span class=\"token punctuation\">,</span> <span class=\"token punctuation\">{</span> <span class=\"token function-variable function\">getValueFromEvent</span><span class=\"token punctuation\">:</span> <span class=\"token punctuation\">(</span><span class=\"token parameter\">value</span><span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\n                <span class=\"token keyword\">if</span> <span class=\"token punctuation\">(</span>value<span class=\"token punctuation\">.</span><span class=\"token function\">match</span><span class=\"token punctuation\">(</span><span class=\"token regex\">/##/</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n                    <span class=\"token keyword\">return</span> value<span class=\"token punctuation\">;</span>\n                <span class=\"token punctuation\">}</span> <span class=\"token keyword\">else</span> <span class=\"token punctuation\">{</span>\n                    <span class=\"token keyword\">return</span> <span class=\"token template-string\"><span class=\"token template-punctuation string\">`</span><span class=\"token string\">## title-</span><span class=\"token interpolation\"><span class=\"token interpolation-punctuation punctuation\">${</span>value<span class=\"token interpolation-punctuation punctuation\">}</span></span><span class=\"token template-punctuation string\">`</span></span><span class=\"token punctuation\">;</span>\n                <span class=\"token punctuation\">}</span>\n            <span class=\"token punctuation\">}</span><span class=\"token punctuation\">}</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">}</span><span class=\"token plain-text\"> />\n            </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Button</span></span> <span class=\"token attr-name\">type</span><span class=\"token attr-value\"><span class=\"token punctuation\">=</span><span class=\"token punctuation\">\"</span>primary<span class=\"token punctuation\">\"</span></span> <span class=\"token attr-name\">onClick</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\n                console<span class=\"token punctuation\">.</span><span class=\"token function\">log</span><span class=\"token punctuation\">(</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>field<span class=\"token punctuation\">.</span><span class=\"token function\">getValues</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n            <span class=\"token punctuation\">}</span><span class=\"token punctuation\">}</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">getValues</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span><span class=\"token class-name\">Button</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n        </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>div</span><span class=\"token punctuation\">></span></span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n<span class=\"token punctuation\">}</span>\n\n\nReactDOM<span class=\"token punctuation\">.</span><span class=\"token function\">render</span><span class=\"token punctuation\">(</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">App</span></span><span class=\"token punctuation\">/></span></span><span class=\"token punctuation\">,</span> mountNode<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span></code></pre></div>"}