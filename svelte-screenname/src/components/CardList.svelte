<script>
    import Card from './Card.svelte';
    export let items = [];
</script>

{#each items as item (item.id)}
    <Card>
        <h2 class="friend-screenname">
            {item.screenname}
        </h2>
    
        <div class="item-child">
                <div class="currently-items">
                    <div class="image">
    
                    </div>
                    <div class="info">
                    <h4>currently</h4>
                    <h3>{item.action}</h3>
                    <div class="currently-title">
                        <p class="title">{item.currently}</p>
                        <p class="platform">{item.platform}</p>
                    </div>
                    </div>
                </div>
    
                <p class="current-opinion">
                    <i class="fa-solid fa-quote-left"></i>
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                </p>
    
                <div class="interaction-bar">
                    <ul>
                        <li class="online">
                        <i class="fa-solid fa-circle"></i>
                        </li>
                        <li>
                        <i class="fa-solid fa-user-plus"></i>
                        </li>
                    </ul>
                </div>
        </div>
    </Card>
{/each}
