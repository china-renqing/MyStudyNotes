# 无障碍

#### 语义化的HTML

* 因为我们在return写jsx的时候，只能拥有一个父级标签，如果没有父级标签的时候，可以使用`React Fragments`来组合各个零散的元素

  * ```jsx
    function ListItem(props) {
      return (
        <dl>
            <Fragment key={item.id}>
              <dt>{item.term}</dt>
              <dd>{item.description}</dd>
            </Fragment>
        </dl>
      );
    }
    ```

  * 当不需要再fragment标签种添加任何prop且工具支持的时候，可以使用短语发：

  * ```jsx
    function ListItem(props) {
      return (
        <>
          <dt>{item.term}</dt>
          <dd>{item.description}</dd>
        </>
      );
    }
    ```

  * 