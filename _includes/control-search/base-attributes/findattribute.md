Represents the base attribute class for the finding attributes.

#### Properties

<div class="member">
    <span class="head"><span class="keyword">public</span> <span class="keyword">int</span></span>
    <h3><span class="body">Index</span><span class="tail"> { <span class="keyword">get</span>; <span class="keyword">set</span>; }</span></h3>
</div>

Gets or sets the index of the control. The default value is `-1`, meaning that the index is not used.

<div class="member">
    <span class="head"><span class="keyword">public</span> <a href="#visibility" class="type">Visibility</a></span>
    <h3><span class="body">Visibility</span><span class="tail"> { <span class="keyword">get</span>; <span class="keyword">set</span>; }</span></h3>
</div>

Gets or sets the visibility. The default value is `Visibility.Visible`.

<div class="member">
    <span class="head"><span class="keyword">public</span> <a href="#scopesource" class="type">ScopeSource</a></span>
    <h3><span class="body">ScopeSource</span><span class="tail"> { <span class="keyword">get</span>; <span class="keyword">set</span>; }</span></h3>
</div>

Gets or sets the scope source. The default value is `ScopeSource.Parent`.

<div class="member">
    <span class="head"><span class="keyword">public</span> <span class="keyword">string</span></span>
    <h3><span class="body">OuterXPath</span><span class="tail"> { <span class="keyword">get</span>; <span class="keyword">set</span>; }</span></h3>
</div>

Gets or sets the outer XPath. The default value is null, meaning that the control is searchable as descendant (using ".//" XPath) in scope source.

<div class="member">
    <span class="head"><span class="keyword">public</span> <span class="type">Type</span></span>
    <h3><span class="body">Strategy</span><span class="tail"> { <span class="keyword">get</span>; <span class="keyword">set</span>; }</span></h3>
</div>

Gets or sets the strategy type for the control search. Strategy type should implement `IComponentScopeLocateStrategy`. The default value is null, meaning that the default strategy of the specific `FindAttribute` should be used.