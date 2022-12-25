<script lang="ts">
    import '../app.scss';
    import '../app.postcss';
    import type PageData = App.PageData;

    const tabk: PageData = ;
</script>

<div class="drawer">
    <input id="my-drawer-3" type="checkbox" class="drawer-toggle"/>
    <div class="drawer-content flex flex-col">
        <!-- Navbar -->
        <div class="w-full navbar bg-base-300">
            <div class="flex-none lg:hidden">
                <label for="my-drawer-3" class="btn btn-square btn-ghost">
                    <button></button>
                    <svg
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            class="inline-block w-6 h-6 stroke-current"
                    >
                        <path
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                stroke-width="2"
                                d="M4 6h16M4 12h16M4 18h16"
                        />
                    </svg
                    >
                </label>
            </div>
            <div class="flex-1 px-2 mx-2 my-class">
                <span class="my-class__hello">Bla</span>Routine App
            </div>
            <div class="flex-none hidden lg:block">
                <ul class="menu menu-horizontal">
                    <!-- Navbar menu content here -->
                    <li><a href="/create">
                        <button class="btn">Create Task</button>
                    </a></li>
                    <li><a href="/settings">
                        <button class="btn">Settings</button>
                    </a></li>
                </ul>
            </div>
        </div>
        <slot/>
    </div>
    <div class="drawer-side">
        <label for="my-drawer-3" class="drawer-overlay"/>
        <ul class="menu p-4 w-80 bg-base-100">
            <!-- Sidebar content here -->
            <li>
                <button class="btn">Create Task</button>
            </li>
            <li>
                <button class="btn">Create Task</button>
            </li>
        </ul>
    </div>
</div>

<style lang="scss">
  .my-class {
    &__hello {
      color: red;
    }
  }
</style>
